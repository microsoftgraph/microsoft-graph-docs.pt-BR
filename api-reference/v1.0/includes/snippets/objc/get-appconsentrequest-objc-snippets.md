---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70bebdb4cce52c8dfee3246d4e7e153bfd006780
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508211"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAppConsentRequest *appConsentRequest = [[MSGraphAppConsentRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```