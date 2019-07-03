---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0dd1960227b746655723acb554aa3773feb3f0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477649"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsDeviceUsageUserDetailList = [[NSMutableArray alloc] init];
        teamsDeviceUsageUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsDeviceUsageUserDetail *teamsDeviceUsageUserDetail = [[MSGraphTeamsDeviceUsageUserDetail alloc] initWithDictionary:[teamsDeviceUsageUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```