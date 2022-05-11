---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ff2199222aa423dab99947f305e5e0ff0a4173f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324043"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Delete()


```