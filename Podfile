using_local_pods = ENV['USE_LOCAL_PODS'] == 'true' || false

platform :ios, '12.0'

# ignore all warnings from all pods
inhibit_all_warnings!

target 'ArisenSwiftiOSExampleApp' do
  use_frameworks!

  if using_local_pods
    pod 'ArisenSwift', :path => '../arisen-swift'
    pod 'ArisenSwiftAbirixSerializationProvider', :path => '../arisen-swift-abirix-serialization-provider'
    pod 'ArisenSwiftSoftkeySignatureProvider', :path => '../arisen-swift-softkey-signature-provider'
    pod 'ArisenSwiftEcc', :path => '../arisen-swift-ecc'
  else
    pod 'ArisenSwift', '~> 0.2.0'
    pod 'ArisenSwiftAbirixSerializationProvider', '~> 0.2.0'
    pod 'ArisenSwiftSoftkeySignatureProvider', '~> 0.2.0'
  end
end
