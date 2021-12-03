---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3fbbd637a6118978edf82c1eef124152c9cee15
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).Patch(nil)


```