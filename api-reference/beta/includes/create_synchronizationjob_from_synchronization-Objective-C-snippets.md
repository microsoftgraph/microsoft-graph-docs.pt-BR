---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60e3f0271b7a794d5a096f3cefb2697a947f1089
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315438"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationJob *synchronizationJob = [[MSGraphSynchronizationJob alloc] init];
[synchronizationJob setTemplateId:@"BoxOutDelta"];

NSError *error;
NSData *synchronizationJobData = [synchronizationJob getSerializedDataWithError:&error];
[urlRequest setHTTPBody:synchronizationJobData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```