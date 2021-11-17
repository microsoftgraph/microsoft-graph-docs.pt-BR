---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abcbf387d50f5e175ed8835f703cb9f07664aed0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamsAppId := "teamsApp-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).Delete(options)


```