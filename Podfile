# Tag default repository
source 'https://github.com/CocoaPods/Specs.git'

inhibit_all_warnings!
use_frameworks!

project 'Tokenary.xcproject'
workspace 'Tokenary.xcworkspace'

# Remote Pod Versions

trustWalletCoreVersion = '~> 2.6.35'
blockiesSwiftVersion = '~> 0.1.2'
kingfisherVersion = '~> 7.1.2' 
composableArchitectureVersion = '~> ' 

set_shared_pods = lambda do
  pod 'Web3Swift.io', :git => 'https://github.com/grachyov/Web3Swift.git', :branch => 'develop'
  pod 'WalletConnect', git: 'https://github.com/grachyov/wallet-connect-swift', branch: 'master'
  pod 'TrustWalletCore', trustWalletCoreVersion
  pod 'BlockiesSwift', blockiesSwiftVersion
  pod 'Kingfisher', kingfisherVersion
end

# App targets

target 'Tokenary' do
  platform :osx, '11.4'
  set_shared_pods.call
end

target 'Tokenary iOS' do
  platform :ios, '15.0'
  set_shared_pods.call
end
