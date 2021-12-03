---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b28cb0286151b472fd87d4fb5d50fab1046ba2bf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287390"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personAnnotationId := "personAnnotation-id"
graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Delete(nil)


```