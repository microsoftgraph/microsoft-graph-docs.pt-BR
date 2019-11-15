---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59bb0a0aec0966f2cc6324ff3338cc92da5cb8bf
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "35705545"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *userList = [[NSMutableArray alloc] init];
        userList = [jsonFinal valueForKey:@"value"];
        MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[userList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```