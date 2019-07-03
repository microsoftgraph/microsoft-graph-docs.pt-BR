---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 978752b38a56763847c160d9fdfb2d3c54bcd6af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518699"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageAppsUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageAppsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageAppsUserCounts *emailAppUsageAppsUserCounts = [[MSGraphEmailAppUsageAppsUserCounts alloc] initWithDictionary:[emailAppUsageAppsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```