use_frameworks!
platform :ios, '12.0'

target 'Ryu_Tests' do
  pod 'Ryu', :path => './'
end

target 'Example' do
  pod 'Ryu', :path => './'
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
  end
end
