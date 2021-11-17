---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1441973ddd8132f43d7fd09a1e7d8198f6decf89ba590824a69f226fd1f78bd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273251"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite?$expand=issues"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphServiceHealth *serviceHealth = [[MSGraphServiceHealth alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```