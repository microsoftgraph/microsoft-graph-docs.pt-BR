---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a63b9df317109c9b44a836b62b86944875271f5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717865"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/securityActions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *securityActionList = [[NSMutableArray alloc] init];
        securityActionList = [jsonFinal valueForKey:@"value"];
        MSGraphSecurityAction *securityAction = [[MSGraphSecurityAction alloc] initWithDictionary:[securityActionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```