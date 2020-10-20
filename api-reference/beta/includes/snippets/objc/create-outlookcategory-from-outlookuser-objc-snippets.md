---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1e7e50d29e10b03412730316d5076cab0f3fc7c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604230"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] init];
[outlookCategory setDisplayName:@"Project expenses"];
[outlookCategory setColor: [MSGraphCategoryColor preset9]];

NSError *error;
NSData *outlookCategoryData = [outlookCategory getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookCategoryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```