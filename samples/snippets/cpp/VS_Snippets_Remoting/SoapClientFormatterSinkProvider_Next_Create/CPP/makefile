all : soapclientformattersinkprovider_next_server.exe soapclientformattersinkprovider_next_client.exe


soapclientformattersinkprovider_next_server.exe : soapclientformattersinkprovider_next_server.cpp soapclientformattersinkprovider_customprovider.dll SoapClientFormatterSinkProvider_Next_Shared.dll
	cl /clr:pure soapclientformattersinkprovider_next_server.cpp

soapclientformattersinkprovider_next_client.exe : soapclientformattersinkprovider_next_client.cpp soapclientformattersinkprovider_customprovider.dll SoapClientFormatterSinkProvider_Next_Shared.dll
	cl /clr:pure soapclientformattersinkprovider_next_client.cpp

soapclientformattersinkprovider_customprovider.dll : soapclientformattersinkprovider_customprovider.cpp
	cl /clr:pure /LD soapclientformattersinkprovider_customprovider.cpp

SoapClientFormatterSinkProvider_Next_Shared.dll : SoapClientFormatterSinkProvider_Next_Shared.cpp
	cl /clr:pure /LD SoapClientFormatterSinkProvider_Next_Shared.cpp
