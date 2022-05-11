---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cf9567dd010fc1ab6edd3d86e525ddbcbda2aa2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323320"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personAnnotationId := "personAnnotation-id"
graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Delete()


```