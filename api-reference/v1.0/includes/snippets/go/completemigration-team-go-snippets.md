---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c464a535d89faf5c5f3271a87c6a63b115f6f372
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325089"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
graphClient.TeamsById(&teamId).CompleteMigration(team-id).Post()


```