---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54642202fa7d87cca46ecc965d665093208b24b1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322312"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/{plan-id}/buckets"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerBucketList = [[NSMutableArray alloc] init];
        plannerBucketList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerBucket *plannerBucket = [[MSGraphPlannerBucket alloc] initWithDictionary:[plannerBucketList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```