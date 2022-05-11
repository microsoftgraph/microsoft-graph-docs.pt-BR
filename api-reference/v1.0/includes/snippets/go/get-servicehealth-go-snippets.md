---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcb22f0c08161f45f1bfd3eac3e92f08d9f3ee63
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324197"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).Get()


```