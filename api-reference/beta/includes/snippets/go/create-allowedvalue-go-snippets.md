---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e03bddda19b966a31ff1a2b440d851a0042cd188
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323236"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAllowedValue()
id := "Alpine"
requestBody.SetId(&id)
isActive := "true"
requestBody.SetIsActive(&isActive)
customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValues().Post(requestBody)


```