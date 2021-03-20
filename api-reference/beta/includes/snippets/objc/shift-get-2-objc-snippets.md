---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2e8da5fd44a3150cee28959b33443abc6861e35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945792"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphShiftPreferences *shiftPreferences = [[MSGraphShiftPreferences alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```