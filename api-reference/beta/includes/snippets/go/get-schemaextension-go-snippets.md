---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59fa8e1e75953908ca9ffadaf623134654c7e392
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

schemaExtensionId := "schemaExtension-id"
result, err := graphClient.SchemaExtensionsById(&schemaExtensionId).Get(options)


```