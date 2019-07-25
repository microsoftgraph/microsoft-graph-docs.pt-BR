---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe938a7141526a6100778ce314af97cf641971cb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724047"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages?$select=sender,subject"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *messageList = [[NSMutableArray alloc] init];
        messageList = [jsonFinal valueForKey:@"value"];
        MSGraphMessage *message = [[MSGraphMessage alloc] initWithDictionary:[messageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```