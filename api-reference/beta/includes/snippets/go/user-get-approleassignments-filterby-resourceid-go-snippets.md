---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad0816d514c4b850ec06f63b06cb737e48aaea45
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "resourceId%20eq%208e881353-1735-45af-af21-ee1344582a4d",
}
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().Get(options)


```