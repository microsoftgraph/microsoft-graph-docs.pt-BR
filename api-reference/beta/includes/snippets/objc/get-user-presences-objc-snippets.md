---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f63cbf8921d88c6ca9650685a5c1b2ba587d0a24c3cebc428940da9acf0f2d4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099373"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPresence *presence = [[MSGraphPresence alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```