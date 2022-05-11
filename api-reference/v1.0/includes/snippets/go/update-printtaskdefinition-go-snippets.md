---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0fd3d382a70d1810b90face5897db33a621ffec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrintTaskDefinition()
displayName := "Test TaskDefinitionName"
requestBody.SetDisplayName(&displayName)
createdBy := msgraphsdk.NewAppIdentity()
requestBody.SetCreatedBy(createdBy)
displayName := "Requesting App Display Name"
createdBy.SetDisplayName(&displayName)
printTaskDefinitionId := "printTaskDefinition-id"
graphClient.Print().TaskDefinitionsById(&printTaskDefinitionId).Patch(requestBody)


```