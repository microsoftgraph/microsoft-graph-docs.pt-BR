---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86cc187f272d2c58b6b2685f984146afeaeda5dd
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842992"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AAMkADIyAAAhrbPWAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTaskList *todoTaskList = [[MSGraphTodoTaskList alloc] init];
[todoTaskList setDisplayName:@"Vacation Plan"];

NSError *error;
NSData *todoTaskListData = [todoTaskList getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskListData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```