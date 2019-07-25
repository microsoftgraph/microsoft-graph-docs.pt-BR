---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1797b1476cba76c163963fc44aab3790ad62918
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710108"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applicationTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *applicationTemplateList = [[NSMutableArray alloc] init];
        applicationTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphApplicationTemplate *applicationTemplate = [[MSGraphApplicationTemplate alloc] initWithDictionary:[applicationTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```