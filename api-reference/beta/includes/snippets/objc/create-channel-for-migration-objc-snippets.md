---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03549682b3042ca409614fc0d0ea64e3f3b4ecce
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753796"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChannel *channel = [[MSGraphChannel alloc] init];
[channel set@microsoft.graph.channelCreationMode:@"migration"];
[channel setDisplayName:@"Architecture Discussion"];
[channel setDescription:@"This channel is where we debate all future architecture plans"];
[channel setMembershipType: [MSGraphChannelMembershipType standard]];
[channel setCreatedDateTime: "2020-03-14T11:22:17.067Z"];

NSError *error;
NSData *channelData = [channel getSerializedDataWithError:&error];
[urlRequest setHTTPBody:channelData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```