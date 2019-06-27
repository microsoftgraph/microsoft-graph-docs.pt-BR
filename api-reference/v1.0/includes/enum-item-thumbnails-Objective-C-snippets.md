---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54f7a7f391a49cf7ac80cc0d422dab3ee0d8cd59
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35321567"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/thumbnails"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *thumbnailSetList = [[NSMutableArray alloc] init];
        thumbnailSetList = [jsonFinal valueForKey:@"value"];
        MSGraphThumbnailSet *thumbnailSet = [[MSGraphThumbnailSet alloc] initWithDictionary:[thumbnailSetList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```