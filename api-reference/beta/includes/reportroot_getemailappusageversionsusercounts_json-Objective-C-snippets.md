---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99a38bb32004aee3c8b7479afbbf5d3f10330638
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35328769"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageVersionsUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageVersionsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageVersionsUserCounts *emailAppUsageVersionsUserCounts = [[MSGraphEmailAppUsageVersionsUserCounts alloc] initWithDictionary:[emailAppUsageVersionsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```