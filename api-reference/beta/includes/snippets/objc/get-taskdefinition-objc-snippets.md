---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05c45f6cf92702d932c5de117096eb0b733b38f11f179a3d6e31b34fd78f7040
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157381"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPrintTaskDefinition *printTaskDefinition = [[MSGraphPrintTaskDefinition alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```