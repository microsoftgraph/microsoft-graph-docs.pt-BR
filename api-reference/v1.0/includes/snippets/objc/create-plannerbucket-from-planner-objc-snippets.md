---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd1fec4233d60ef3dbb4a6280d2f2e019c760063
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621570"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/buckets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerBucket *plannerBucket = [[MSGraphPlannerBucket alloc] init];
[plannerBucket setName:@"Advertising"];
[plannerBucket setPlanId:@"xqQg5FS2LkCp935s-FIFm2QAFkHM"];
[plannerBucket setOrderHint:@" !"];

NSError *error;
NSData *plannerBucketData = [plannerBucket getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerBucketData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```