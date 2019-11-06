---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b38305d496616aa7cf130bee82ad12b122e986b1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996892"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/phones"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *itemPhoneList = [[NSMutableArray alloc] init];
        itemPhoneList = [jsonFinal valueForKey:@"value"];
        MSGraphItemPhone *itemPhone = [[MSGraphItemPhone alloc] initWithDictionary:[itemPhoneList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```