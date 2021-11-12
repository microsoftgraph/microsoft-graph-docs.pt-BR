---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53f2a580a9d31b21137fa44368825ffb7a07afd28b60859d6eab7256946c587b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899659"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA="]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOutlookTaskGroup *outlookTaskGroup = [[MSGraphOutlookTaskGroup alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```