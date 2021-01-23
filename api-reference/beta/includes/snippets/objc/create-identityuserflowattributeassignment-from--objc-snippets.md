---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d53779ce1dabc3a13d3b6fd4874b04640d2bcbc9
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945640"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlowAttributeAssignment *identityUserFlowAttributeAssignment = [[MSGraphIdentityUserFlowAttributeAssignment alloc] init];
[identityUserFlowAttributeAssignment setIsOptional: false];
[identityUserFlowAttributeAssignment setRequiresVerification: false];
[identityUserFlowAttributeAssignment setUserInputType: [MSGraphIdentityUserFlowAttributeInputType textBox]];
[identityUserFlowAttributeAssignment setDisplayName:@"Shoe size"];
NSMutableArray *userAttributeValuesList = [[NSMutableArray alloc] init];
[identityUserFlowAttributeAssignment setUserAttributeValues:userAttributeValuesList];
MSGraphIdentityUserFlowAttribute *userAttribute = [[MSGraphIdentityUserFlowAttribute alloc] init];
[userAttribute setId:@"extension_guid_shoeSize"];
[identityUserFlowAttributeAssignment setUserAttribute:userAttribute];

NSError *error;
NSData *identityUserFlowAttributeAssignmentData = [identityUserFlowAttributeAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityUserFlowAttributeAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```