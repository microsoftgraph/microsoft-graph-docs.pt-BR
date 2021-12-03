---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b177b53e0d373ba0a638f8dc49ba5618f2ccc46
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286099"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

customSecurityAttributeDefinitionId := "customSecurityAttributeDefinition-id"
result, err := graphClient.Directory().CustomSecurityAttributeDefinitionsById(&customSecurityAttributeDefinitionId).AllowedValues().Get(nil)


```