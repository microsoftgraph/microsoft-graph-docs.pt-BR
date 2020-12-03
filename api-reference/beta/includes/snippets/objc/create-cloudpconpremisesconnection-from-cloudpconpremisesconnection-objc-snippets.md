---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3782d6d8f7ca793989c42867646c270c531285ef
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523383"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/onPremisesConnections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcOnPremisesConnection *cloudPcOnPremisesConnection = [[MSGraphCloudPcOnPremisesConnection alloc] init];
[cloudPcOnPremisesConnection setDisplayName:@"Display Name value"];
[cloudPcOnPremisesConnection setSubscriptionId:@"0ac520ee-14c0-480f-b6c9-0a90c585ffff"];
[cloudPcOnPremisesConnection setSubscriptionName:@"Subscription Name value"];
[cloudPcOnPremisesConnection setAdDomainName:@"Active Directory Domain Name value"];
[cloudPcOnPremisesConnection setAdDomainUsername:@"Active Directory Domain User Name value"];
[cloudPcOnPremisesConnection setOrganizationalUnit:@"Organization Unit value"];
[cloudPcOnPremisesConnection setResourceGroupId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG"];
[cloudPcOnPremisesConnection setVirtualNetworkId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet"];
[cloudPcOnPremisesConnection setSubnetId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"];

NSError *error;
NSData *cloudPcOnPremisesConnectionData = [cloudPcOnPremisesConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcOnPremisesConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```