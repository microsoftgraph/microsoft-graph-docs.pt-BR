---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6c990ca2f3c9444d6cc194310cd213697a48f9e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "displayName,userPrincipalName,signInActivity",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```