---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00548e8b3cfae905e44d7829482c2298bb4a9b3f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526088"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *availability = @"DoNotDisturb";
payloadDictionary[@"availability"] = availability;

NSString *activity = @"DoNotDisturb";
payloadDictionary[@"activity"] = activity;

NSString *expirationDuration = @"PT8H";
payloadDictionary[@"expirationDuration"] = expirationDuration;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```