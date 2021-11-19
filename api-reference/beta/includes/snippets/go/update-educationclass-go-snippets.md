---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6bcf819858d8b856f3fb38b210ded4579e832b1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Patch(options)


```