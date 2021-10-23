---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab91e128a0a9ec5598889da83000250359b58c6ea7a57b24bbd5ad8b30f507d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272148"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/continuousAccessEvaluationPolicy"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphContinuousAccessEvaluationPolicy *continuousAccessEvaluationPolicy = [[MSGraphContinuousAccessEvaluationPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```