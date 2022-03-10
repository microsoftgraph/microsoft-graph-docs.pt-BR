---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f943668681a5b453ee75e0246f5c527f9c57a542
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

schemaExtensionId := "schemaExtension-id"
result, err := graphClient.SchemaExtensionsById(&schemaExtensionId).Delete(nil)


```