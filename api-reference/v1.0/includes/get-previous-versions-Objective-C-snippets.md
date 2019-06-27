---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c919f3d59dd15585bd106b16e42728ca32bebf85
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314453"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/versions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *driveItemVersionList = [[NSMutableArray alloc] init];
        driveItemVersionList = [jsonFinal valueForKey:@"value"];
        MSGraphDriveItemVersion *driveItemVersion = [[MSGraphDriveItemVersion alloc] initWithDictionary:[driveItemVersionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```