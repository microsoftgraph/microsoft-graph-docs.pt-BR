---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb3efe1b89e1722f0037390078b034668324e96b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477188"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getMailboxUsageDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *mailboxUsageDetailList = [[NSMutableArray alloc] init];
        mailboxUsageDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphMailboxUsageDetail *mailboxUsageDetail = [[MSGraphMailboxUsageDetail alloc] initWithDictionary:[mailboxUsageDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```