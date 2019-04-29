using_local_pods = true

unless using_local_pods
  source 'https://github.com/EOSIO/eosio-swift-pod-specs.git'
  source 'https://github.com/CocoaPods/Specs.git'
end

platform :ios, '12.0'

# ignore all warnings from all pods
inhibit_all_warnings!

target 'EosioSwiftiOSExampleApp' do
  use_frameworks!

  if using_local_pods
    pod 'EosioSwift', :path => '../eosio-swift'
    pod 'EosioSwiftAbieosSerializationProvider', :path => '../eosio-swift-abieos-serialization-provider'
    pod 'EosioSwiftSoftkeySignatureProvider', :path => '../eosio-swift-softkey-signature-provider'
    pod 'EosioSwiftEcc', :path => '../eosio-swift-ecc'
  else
    pod 'EosioSwift', '~> 0.0.2'
    pod 'EosioSwiftAbieosSerializationProvider', '~> 0.0.3'
    pod 'EosioSwiftSoftkeySignatureProvider', '~> 0.0.2'
  end
end
