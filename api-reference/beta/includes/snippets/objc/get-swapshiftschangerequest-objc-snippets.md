---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be0d93e0a7c5dd720d1abe4aaa8281e51a2853e9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865043"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/swapShiftsChangeRequests"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *swapShiftsChangeRequestList = [[NSMutableArray alloc] init];
        swapShiftsChangeRequestList = [jsonFinal valueForKey:@"value"];
        MSGraphSwapShiftsChangeRequest *swapShiftsChangeRequest = [[MSGraphSwapShiftsChangeRequest alloc] initWithDictionary:[swapShiftsChangeRequestList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```