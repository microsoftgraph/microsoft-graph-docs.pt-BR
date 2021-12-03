---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0133174262b2af6569ba09dd498e185c300b3c24
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287306"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
teamsAppDefinitionId := "teamsAppDefinition-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).AppDefinitionsById(&teamsAppDefinitionId).OutlineIcon().HostedContent().$value().Get(nil)


```