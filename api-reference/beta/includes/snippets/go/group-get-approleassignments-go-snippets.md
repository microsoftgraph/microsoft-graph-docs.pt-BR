---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c70872442dff5f1c6edb094024bafecde2c3d21f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324676"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AppRoleAssignments().Get()


```