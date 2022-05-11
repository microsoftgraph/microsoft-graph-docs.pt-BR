---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5aacd55baedb3fa5afaf1a8f326eb9060b49841
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325035"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Planner().All().Delta()().Get()


```