---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66241002bba302fd38e375e239c6ed9729b30a38
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personWebsiteId := "personWebsite-id"
graphClient.Me().Profile().WebsitesById(&personWebsiteId).Delete()


```