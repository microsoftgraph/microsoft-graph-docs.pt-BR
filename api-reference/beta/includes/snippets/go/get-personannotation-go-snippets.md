---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40f07d360cf6f2e89f1e539c9065f2a4703f861c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287310"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personAnnotationId := "personAnnotation-id"
result, err := graphClient.Me().Profile().NotesById(&personAnnotationId).Get(nil)


```