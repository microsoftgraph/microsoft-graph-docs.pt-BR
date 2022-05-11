---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0b91610ca293caf5f8019ca7d376b8dda09a2ec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325555"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
graphClient.TeamsById(&teamId).Unarchive(team-id).Post()


```