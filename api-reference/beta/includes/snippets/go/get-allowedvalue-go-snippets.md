---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cdb4b6330910f6024a25cf6d44dc10195236be8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285875"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
allowedValueId := "allowedValue-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValuesById(&allowedValueId).Get(nil)


```