---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81a5092555db445aedadde8e5b55c967b01d7306
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322815"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttributeSet()
id := "Engineering"
requestBody.SetId(&id)
description := "Attributes for engineering team"
requestBody.SetDescription(&description)
maxAttributesPerSet := int32(25)
requestBody.SetMaxAttributesPerSet(&maxAttributesPerSet)
result, err := graphClient.Directory().AttributeSets().Post(requestBody)


```