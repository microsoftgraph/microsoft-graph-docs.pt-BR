---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 924b2340a6364f3a3f9150783d416074ec950292
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35317764"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedApproval"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedApproval *privilegedApproval = [[MSGraphPrivilegedApproval alloc] init];
[privilegedApproval setUserId:@"userId-value"];
[privilegedApproval setRoleId:@"roleId-value"];
[privilegedApproval setApprovalType:@"approvalType-value"];
[privilegedApproval setApprovalState: [MSGraphApprovalState pending]];
[privilegedApproval setApprovalDuration:@"datetime-value"];

NSError *error;
NSData *privilegedApprovalData = [privilegedApproval getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedApprovalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```