---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0f4d9833c0e337e429ad069e6c82ebfd141573d
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559127"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrationQuestion *meetingRegistrationQuestion = [[MSGraphMeetingRegistrationQuestion alloc] init];
[meetingRegistrationQuestion setDisplayName:@"What's your job position?"];
[meetingRegistrationQuestion setIsRequired: false];
[meetingRegistrationQuestion setAnswerInputType: [MSGraphAnswerInputType text]];

NSError *error;
NSData *meetingRegistrationQuestionData = [meetingRegistrationQuestion getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrationQuestionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```