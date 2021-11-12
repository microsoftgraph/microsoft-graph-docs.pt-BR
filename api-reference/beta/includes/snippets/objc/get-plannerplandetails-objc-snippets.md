---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72c96bab6e092d387236983d2c75c6b93d077f899d45e2e028d155b1c90e8626
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327806"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPlannerPlanDetails *plannerPlanDetails = [[MSGraphPlannerPlanDetails alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```