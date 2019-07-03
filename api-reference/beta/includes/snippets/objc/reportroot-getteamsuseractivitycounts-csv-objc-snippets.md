---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf449e05a97b2f74ba5b4117d904bde575d04ae4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518584"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsUserActivityCountsList = [[NSMutableArray alloc] init];
        teamsUserActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsUserActivityCounts *teamsUserActivityCounts = [[MSGraphTeamsUserActivityCounts alloc] initWithDictionary:[teamsUserActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```