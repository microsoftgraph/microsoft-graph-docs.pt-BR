---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3987495c751d1d4327f0fd8deb2d1e297f6cbe4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318070"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/conversations"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conversationList = [[NSMutableArray alloc] init];
        conversationList = [jsonFinal valueForKey:@"value"];
        MSGraphConversation *conversation = [[MSGraphConversation alloc] initWithDictionary:[conversationList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```