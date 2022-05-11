---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60d332a1b61e71f38ad24d54ac0ecec79c4257a3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Outlook().SupportedTimeZones()().Get()


```