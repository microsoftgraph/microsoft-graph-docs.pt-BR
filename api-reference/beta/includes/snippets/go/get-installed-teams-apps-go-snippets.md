---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc691b89d24ddc1203e9daae4243a3f40083188b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026093"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
teamsAppInstallationId := "teamsAppInstallation-id"
result, err := graphClient.TeamsById(&teamId).InstalledAppsById(&teamsAppInstallationId).Get(options)


```