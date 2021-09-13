---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37056b10cd1d4278b71437452c3c6da53600344c25d5a018a08e528a7060c58f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327810"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/shares/{shareIdOrEncodedSharingUrl}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSharedDriveItem *sharedDriveItem = [[MSGraphSharedDriveItem alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```