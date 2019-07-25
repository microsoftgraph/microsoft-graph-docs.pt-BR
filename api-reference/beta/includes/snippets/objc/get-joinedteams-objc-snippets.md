---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78ce34e08bcd4c6747c1aa0c2f84b1396fccd9c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867268"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/joinedTeams"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamList = [[NSMutableArray alloc] init];
        teamList = [jsonFinal valueForKey:@"value"];
        MSGraphTeam *team = [[MSGraphTeam alloc] initWithDictionary:[teamList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```