---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62986fc5a7317c7728fd85323d8755c5c793bd1c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InvalidateAllRefreshTokens().Post()


```