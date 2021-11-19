---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6313e801f21556863399c81d2f030857b3f392ae
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089432"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamsAppId := "teamsApp-id"
graphClient.AppCatalogs().TeamsAppsById(&teamsAppId).Delete(options)


```