---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 401d4d896fd85d33835d0707d3f6957bb2c5c6aa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60995201"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/softwareOathMethods"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphSoftwareOathAuthenticationMethod *softwareOathAuthenticationMethod = [[MSGraphSoftwareOathAuthenticationMethod alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```