---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 157bde4e4f333fd1d7db9f7510ce296cb6880746
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991406"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewScopedRoleMembership()
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
roleMemberInfo := msgraphsdk.NewIdentity()
requestBody.SetRoleMemberInfo(roleMemberInfo)
id := "id-value"
roleMemberInfo.SetId(&id)
options := &msgraphsdk.ScopedRoleMembersRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembers().Post(options)


```