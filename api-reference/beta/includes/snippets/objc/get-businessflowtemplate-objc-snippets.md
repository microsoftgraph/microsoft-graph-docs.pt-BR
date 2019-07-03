---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 188aa5fa1bcb7bde575f20300d6c4ed05e130368
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499031"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/businessFlowTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *businessFlowTemplateList = [[NSMutableArray alloc] init];
        businessFlowTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphBusinessFlowTemplate *businessFlowTemplate = [[MSGraphBusinessFlowTemplate alloc] initWithDictionary:[businessFlowTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```