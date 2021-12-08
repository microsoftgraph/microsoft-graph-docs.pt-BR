---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ea2f44024ea234bb01f813358c7642349a5e87b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341815"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackage *accessPackage = [[MSGraphAccessPackage alloc] init];
[accessPackage setDisplayName:@"sales reps"];
[accessPackage setDescription:@"outside sales representatives"];
[accessPackage setIsHidden: false];
MSGraphAccessPackageCatalog *catalog = [[MSGraphAccessPackageCatalog alloc] init];
[catalog setId:@"66584aae-98bb-48cc-9458-7bee5d2a6577"];
[accessPackage setCatalog:catalog];

NSError *error;
NSData *accessPackageData = [accessPackage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```