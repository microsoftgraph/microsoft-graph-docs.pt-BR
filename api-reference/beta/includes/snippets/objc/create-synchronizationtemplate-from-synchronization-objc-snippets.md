---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ff771756ea3175d7e85653fddb017c6513a5a27
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614374"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/synchronization/templates"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationTemplate *synchronizationTemplate = [[MSGraphSynchronizationTemplate alloc] init];
[synchronizationTemplate setId:@"SCIM-Test1"];
[synchronizationTemplate setApplicationId:@"{id}"];
[synchronizationTemplate setFactoryTag:@"CustomSCIM"];

NSError *error;
NSData *synchronizationTemplateData = [synchronizationTemplate getSerializedDataWithError:&error];
[urlRequest setHTTPBody:synchronizationTemplateData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```