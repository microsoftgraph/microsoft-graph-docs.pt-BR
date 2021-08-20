---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66492cdf40137adb2ca9b20d079afa044218bb66faa8761a50fdccdc4261d577
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215572"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] init];
[onlineMeeting setStartDateTime: "2020-09-09T21:33:30.8546353+00:00"];
[onlineMeeting setEndDateTime: "2020-09-09T22:03:30.8566356+00:00"];
[onlineMeeting setSubject:@"Patch Meeting Subject"];

NSError *error;
NSData *onlineMeetingData = [onlineMeeting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onlineMeetingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```