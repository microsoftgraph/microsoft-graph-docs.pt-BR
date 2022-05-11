---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42f80d8b1506a690ed9eb5762da4e77b7ef4329e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324838"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPatentId := "itemPatent-id"
result, err := graphClient.Me().Profile().PatentsById(&itemPatentId).Get()


```