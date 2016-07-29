source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '9.0'
use_frameworks!
inhibit_all_warnings!

def required_pods

pod 'FontAwesomeKit'
pod 'Siesta/Alamofire' , '1.0-beta.6'
pod 'ChameleonFramework/Swift'
pod 'DZNEmptyDataSet'
pod 'PermissionScope'
pod 'IQKeyboardManagerSwift'
pod 'SDWebImage'
pod 'Analytics'
pod 'Fabric'
pod 'Crashlytics'
pod 'CryptoSwift'
pod 'KeychainAccess'
pod 'Segment-Localytics'
pod 'SwiftyBeaver'
pod 'Segment-Appboy'

end

target "SegmentAppboyFail" do
    required_pods
    post_install do |installer|
        installer.pods_project.targets.each do |target|
            target.build_configurations.each do |config|
                config.build_settings['ENABLE_BITCODE'] = 'NO'
            end
        end
    end
end

