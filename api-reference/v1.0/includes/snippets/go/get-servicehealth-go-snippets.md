---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11a922ba7d3efc04a984af4e96165dd05ebc9c90
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013065"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).Get(options)


```