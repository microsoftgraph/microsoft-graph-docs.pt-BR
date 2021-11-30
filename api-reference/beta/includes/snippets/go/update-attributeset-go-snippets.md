---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5887c14403f8a0df1fd51b4b12c394c97affa087
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223529"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttributeSet()
description := "Attributes for engineering team"
requestBody.SetDescription(&description)
maxAttributesPerSet := int32(20)
requestBody.SetMaxAttributesPerSet(&maxAttributesPerSet)
options := &msgraphsdk.AttributeSetRequestBuilderPatchOptions{
    Body: requestBody,
}
attributeSetId := "attributeSet-id"
graphClient.Directory().AttributeSetsById(&attributeSetId).Patch(options)


```