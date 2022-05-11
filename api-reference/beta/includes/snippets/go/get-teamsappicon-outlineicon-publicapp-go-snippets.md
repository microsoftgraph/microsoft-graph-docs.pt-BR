---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23143a5dc42a10fb1b549c2f0e7fda59edbb4118
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323431"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
result, err := graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).OutlineIcon().Get()


```