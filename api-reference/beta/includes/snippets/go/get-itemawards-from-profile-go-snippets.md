---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95e91cbbbdb2ba2856dacb4bda22eb2a7c3add2a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323865"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Awards().Get()


```