---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a37d2c83748e262d71f2567303ae67c1bc60fcaf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

schemaExtensionId := "schemaExtension-id"
graphClient.SchemaExtensionsById(&schemaExtensionId).Delete(nil)


```