---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d928994416660b65169deb4f509187b7027c6e7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287179"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Upgrade().Post(nil)


```