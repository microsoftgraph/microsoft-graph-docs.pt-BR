---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a7f5c121747fab5352b8621d457396d642c822f
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689634"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphConversationMember *values = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[values setRoles:rolesList];
[valuesList addObject: values];
MSGraphConversationMember *values = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[values setRoles:rolesList];
[valuesList addObject: values];
payloadDictionary[@"values"] = valuesList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```