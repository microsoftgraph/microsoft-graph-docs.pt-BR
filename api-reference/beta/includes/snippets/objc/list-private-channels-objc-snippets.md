---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb38748c37f332ebc5a454d5e2d5e03889062992
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402324"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/channels?$filter=membershipType%20eq%20'private'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *channelList = [[NSMutableArray alloc] init];
        channelList = [jsonFinal valueForKey:@"value"];
        MSGraphChannel *channel = [[MSGraphChannel alloc] initWithDictionary:[channelList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```