---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da3f35151e9cda7de3a1b1f10e264a5fd8683ac4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61020366"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/softwareOathMethods/b172893e-893e-b172-3e89-72b13e8972b1"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSoftwareOathAuthenticationMethod *softwareOathAuthenticationMethod = [[MSGraphSoftwareOathAuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```