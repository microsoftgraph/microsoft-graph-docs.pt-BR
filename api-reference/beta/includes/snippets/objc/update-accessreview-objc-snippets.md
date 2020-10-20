---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 550f33e7dddda6e4b6a2134e5dd7611f8fab1f78
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619717"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/accessReviews/006111db-0810-4494-a6df-904d368bd81b"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReview *accessReview = [[MSGraphAccessReview alloc] init];
[accessReview setDisplayName:@"TestReview new name"];

NSError *error;
NSData *accessReviewData = [accessReview getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```