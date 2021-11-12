---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58bb1183813e52aba55805276ab12bdfb6822e9e613daa30c7f2af470730316b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159639"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/{printerId}/taskTriggers/{taskTriggerId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPrintTaskTrigger *printTaskTrigger = [[MSGraphPrintTaskTrigger alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```