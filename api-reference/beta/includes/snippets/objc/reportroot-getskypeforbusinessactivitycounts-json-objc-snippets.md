---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34ba2a3e6b45ce4b13f3a50a01ded74972152634
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476352"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessActivityCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessActivityCounts *skypeForBusinessActivityCounts = [[MSGraphSkypeForBusinessActivityCounts alloc] initWithDictionary:[skypeForBusinessActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```