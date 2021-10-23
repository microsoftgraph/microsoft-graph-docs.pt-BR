---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 749a7313310a017eeab57f171e4a2fbc39580c84
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562723"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"0" forHTTPHeaderField:@"Accept-Language"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOrganizationalBranding *organizationalBranding = [[MSGraphOrganizationalBranding alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```