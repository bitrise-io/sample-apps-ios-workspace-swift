# Uncomment the next line to define a global platform for your project
# platform :ios, '14.7'

target 'sample-apps-ios-workspace-swift' do
  use_frameworks!

  # Pods for sample-apps-ios-workspace-swift
  pod 'SnapKit', '~> 4.0'

  target 'sample-apps-ios-workspace-swiftTests' do
    inherit! :search_paths
    # Pods for testing
    pod 'SnapKit', '~> 4.0'
  end

  target 'sample-apps-ios-workspace-swiftUITests' do
    inherit! :search_paths
    # Pods for testing
    pod 'SnapKit', '~> 4.0'
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
    end
  end
end
