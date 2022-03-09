---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef56f6506f23642abdd3e4e6e7d4bcb0fbf57327dfeaf2b71b52a81d9bf792ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213585"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/informationprotection/policy/labels/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphInformationProtectionLabel *informationProtectionLabel = [[MSGraphInformationProtectionLabel alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```