---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ee94b830500cfad73fac6e319d730136b1b58eb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212233"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).IncomingChannels().Get(nil)


```