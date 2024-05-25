# Uncomment the next line to define a global platform for your project
 platform :ios, '14.0'

target 'LLDebugToolDemo' do
  # Uncomment the next line if you're using Swift or would like to use dynamic frameworks
  # use_frameworks!

  # Pods for LLDebugToolDemo

  # Request
  pod 'FMDB','~> 2.0',:inhibit_warnings => true

  # Only for demo
  pod 'AFNetworking'

  target 'LLDebugToolDemoTests' do
    inherit! :search_paths
    # Pods for testing
    
    # Request
    pod 'FMDB'
    
    # Only for demo
    pod 'AFNetworking'
    
  end

  target 'LLDebugToolDemoUITests' do
    inherit! :search_paths
    # Pods for testing
    
    # Request
    pod 'FMDB'
    
    # Only for demo
    pod 'AFNetworking'
    
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['APPLICATION_EXTENSION_API_ONLY'] = 'NO'
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
    end
  end
end
