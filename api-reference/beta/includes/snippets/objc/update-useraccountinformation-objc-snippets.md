---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0adc4bd85740936ba5c0327172f080a5a2a2d86c7c2472035dc66f666117cd8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899257"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/account/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserAccountInformation *userAccountInformation = [[MSGraphUserAccountInformation alloc] init];
[userAccountInformation setCountryCode:@"NO"];

NSError *error;
NSData *userAccountInformationData = [userAccountInformation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userAccountInformationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```