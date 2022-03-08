---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8a0922418b9c1b059e2fcc23be1da35c0516e29
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336491"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/crossTenantAccessPolicy/default"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCrossTenantAccessPolicyConfigurationDefault *crossTenantAccessPolicyConfigurationDefault = [[MSGraphCrossTenantAccessPolicyConfigurationDefault alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```