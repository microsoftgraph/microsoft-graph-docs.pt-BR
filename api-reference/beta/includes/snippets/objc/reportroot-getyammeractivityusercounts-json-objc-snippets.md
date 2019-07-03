---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c70f04f92d99acca0333e8fcdff98886c9b8a541
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519338"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerActivitySummaryList = [[NSMutableArray alloc] init];
        yammerActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerActivitySummary *yammerActivitySummary = [[MSGraphYammerActivitySummary alloc] initWithDictionary:[yammerActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```