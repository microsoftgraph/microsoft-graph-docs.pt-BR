---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c81c4b7351c8416b24d0cd7058b26c7ca0f250ff
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203686"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Teamwork().AssociatedTeams().Get(nil)


```