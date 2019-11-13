---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60c7d4cb998e2196e963e525620899d73a04cd1b
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302781"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/audioRoutingGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *audioRoutingGroupList = [[NSMutableArray alloc] init];
        audioRoutingGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphAudioRoutingGroup *audioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] initWithDictionary:[audioRoutingGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```