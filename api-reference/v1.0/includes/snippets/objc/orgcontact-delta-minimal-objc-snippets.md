---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daec37afa52e919cbcc909cd79ad9ded7f5aed8d
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082127"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/contacts/delta?$select=displayName,jobTitle,mail"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"return=minimal" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOrgContact *orgContact = [[MSGraphOrgContact alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```