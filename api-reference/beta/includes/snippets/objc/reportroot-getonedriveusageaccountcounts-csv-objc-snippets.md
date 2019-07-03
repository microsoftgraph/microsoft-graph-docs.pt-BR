---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa18e5ad7f86c20d51fa0db9da8122658a6aa4fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475917"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageAccountCountsList = [[NSMutableArray alloc] init];
        oneDriveUsageAccountCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageAccountCounts *oneDriveUsageAccountCounts = [[MSGraphOneDriveUsageAccountCounts alloc] initWithDictionary:[oneDriveUsageAccountCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```