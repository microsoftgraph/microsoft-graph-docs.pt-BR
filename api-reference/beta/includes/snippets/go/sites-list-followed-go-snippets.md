---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2b9fef3dbf93bbbaa30a092571287aa8e95de17
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324384"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().FollowedSites().Get()


```