---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38953fcd765cf3dc06f09f30247718ae9d84f74c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334685"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProtection/riskyServicePrincipals/9089a539-a539-9089-39a5-899039a58990"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRiskyServicePrincipal *riskyServicePrincipal = [[MSGraphRiskyServicePrincipal alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```