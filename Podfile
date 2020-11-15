platform :ios, '13.0'

target 'ChatDemo' do
  use_frameworks!

  # Pods for ChatDemo
  pod 'Firebase/Auth'
  pod 'Firebase/Firestore'
  pod 'GoogleSignIn'
  pod 'IQKeyboardManagerSwift'
  
  post_install do |installer|
       installer.pods_project.targets.each do |target|
           target.build_configurations.each do |config|
               config.build_settings['DEBUG_INFORMATION_FORMAT'] = 'dwarf'
               config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
               config.build_settings['ONLY_ACTIVE_ARCH'] = 'YES'
           end
       end
    end

end
