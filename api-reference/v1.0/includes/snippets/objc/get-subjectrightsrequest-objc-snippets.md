---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73c1f2e3c6b58b9b2910d582e9ad348e96e45039
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687641"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privacy/subjectRightsRequests/{subjectRightsRequestId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSubjectRightsRequest *subjectRightsRequest = [[MSGraphSubjectRightsRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```