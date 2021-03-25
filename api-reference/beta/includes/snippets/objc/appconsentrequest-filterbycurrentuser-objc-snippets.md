---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3426509c890e3e7a570737e73002c1cf1ce21cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201743"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status%20eq%20'InProgress')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAppConsentRequest *appConsentRequest = [[MSGraphAppConsentRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```