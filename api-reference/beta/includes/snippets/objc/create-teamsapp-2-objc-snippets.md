---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4549ace76e455597df349bc44b56647e749beb4b6a1f102908dd9b041cc2cbe6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375917"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/appCatalogs/teamsApps?requiresReview=true"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/zip" forHTTPHeaderField:@"Content-Type"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```