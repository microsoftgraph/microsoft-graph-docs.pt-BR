---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5cc2dd1ac3501af729963b43f4fe2e9b136252cadfd66de51583d884be2f75a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102788"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChat *chat = [[MSGraphChat alloc] init];
[chat setTopic:@"Group chat title update"];

NSError *error;
NSData *chatData = [chat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```