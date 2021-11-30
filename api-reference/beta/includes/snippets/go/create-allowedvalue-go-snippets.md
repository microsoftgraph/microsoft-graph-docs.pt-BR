---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bafaf982d46468d5d26e246da305fdff6ba348e2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224497"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAllowedValue()
id := "Alpine"
requestBody.SetId(&id)
isActive := "true"
requestBody.SetIsActive(&isActive)
options := &msgraphsdk.AllowedValuesRequestBuilderPostOptions{
    Body: requestBody,
}
customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValues().Post(options)


```