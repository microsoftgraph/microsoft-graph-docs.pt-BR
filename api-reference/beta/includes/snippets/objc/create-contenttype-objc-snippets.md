---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5994c1cd04973c799194eaec384177393be28ce
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202043"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{id}/contentTypes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContentType *contentType = [[MSGraphContentType alloc] init];
[contentType setName:@"docSet"];
[contentType setDescription:@"custom docset"];
MSGraphContentType *base = [[MSGraphContentType alloc] init];
[base setName:@"Document Set"];
[base setId:@"0x0120D520"];
[contentType setBase:base];
[contentType setGroup:@"Document Set Content Types"];

NSError *error;
NSData *contentTypeData = [contentType getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contentTypeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```