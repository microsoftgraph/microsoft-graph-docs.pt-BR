---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 315c664def343a8758292b07070131c281977caf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715415"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"Bearer {Token}" forHTTPHeaderField:@"Authorization"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSynchronizationSchema *synchronizationSchema = [[MSGraphSynchronizationSchema alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```