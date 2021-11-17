---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d773d9be6da888b0fd8a00b686dd2fceee551cbb78cfb3963e4ee2b93a847e2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216252"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWindowsHelloForBusinessAuthenticationMethod *windowsHelloForBusinessAuthenticationMethod = [[MSGraphWindowsHelloForBusinessAuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```