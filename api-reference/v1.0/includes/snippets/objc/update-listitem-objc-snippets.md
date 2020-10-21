---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7508471098d87e5d4d0636b46397623e1c06b146
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611761"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items/{item-id}/fields"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFieldValueSet *fieldValueSet = [[MSGraphFieldValueSet alloc] init];
[fieldValueSet setColor:@"Fuchsia"];
[fieldValueSet setQuantity: 934];

NSError *error;
NSData *fieldValueSetData = [fieldValueSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:fieldValueSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```