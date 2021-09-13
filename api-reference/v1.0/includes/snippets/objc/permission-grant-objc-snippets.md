---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebd6d320653ffc3f5078148ca18e1a0ac01df60d5828ffacd4cab2dfae223808
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158092"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/shares/{encoded-sharing-url}/permission/grant"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *recipientsList = [[NSMutableArray alloc] init];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipients setEmail:@"john@contoso.com"];
[recipientsList addObject: recipients];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipients setEmail:@"ryan@external.com"];
[recipientsList addObject: recipients];
payloadDictionary[@"recipients"] = recipientsList;

NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"read"];
payloadDictionary[@"roles"] = rolesList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```