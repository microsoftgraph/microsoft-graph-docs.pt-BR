---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4504736dabc1c2a3f35884bceb27f0ebd4ba851dda7ed866ec6fcbed53a08b47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271898"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignments/{id}/makePermanent"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *reason = @"reason-value";
payloadDictionary[@"reason"] = reason;

NSString *ticketNumber = @"ticketNumber-value";
payloadDictionary[@"ticketNumber"] = ticketNumber;

NSString *ticketSystem = @"ticketSystem-value";
payloadDictionary[@"ticketSystem"] = ticketSystem;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```