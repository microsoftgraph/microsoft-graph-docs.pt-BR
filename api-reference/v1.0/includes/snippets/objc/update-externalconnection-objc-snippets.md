---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b602f2016c259e0e71d18011c64fe34089052c889f2d54cfae8e4c1b5caa3214
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376728"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalConnection *externalConnection = [[MSGraphExternalConnectorsExternalConnection alloc] init];
[externalConnection setName:@"Contoso HR Service Tickets"];
[externalConnection setDescription:@"Connection to index HR service tickets"];

NSError *error;
NSData *externalConnectionData = [externalConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```