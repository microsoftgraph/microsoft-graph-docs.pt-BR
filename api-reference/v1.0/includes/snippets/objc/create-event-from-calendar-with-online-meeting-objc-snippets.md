---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da8c21a8a05f6524b38c07a5eb496ff393614a50
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771129"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendars/AAMkAGViNDU9zAAAAAGtlAAA=/events"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEvent *event = [[MSGraphEvent alloc] init];
[event setSubject:@"Let's go for lunch"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Does next month work for you?"];
[event setBody:body];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2019-03-10T12:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[event setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2019-03-10T14:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[event setEnd:end];
MSGraphLocation *location = [[MSGraphLocation alloc] init];
[location setDisplayName:@"Harry's Bar"];
[event setLocation:location];
NSMutableArray *attendeesList = [[NSMutableArray alloc] init];
MSGraphAttendee *attendees = [[MSGraphAttendee alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"adelev@contoso.onmicrosoft.com"];
[emailAddress setName:@"Adele Vance"];
[attendees setEmailAddress:emailAddress];
[attendees setType: [MSGraphAttendeeType required]];
[attendeesList addObject: attendees];
[event setAttendees:attendeesList];
[event setIsOnlineMeeting: true];
[event setOnlineMeetingProvider: [MSGraphOnlineMeetingProviderType teamsForBusiness]];

NSError *error;
NSData *eventData = [event getSerializedDataWithError:&error];
[urlRequest setHTTPBody:eventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```