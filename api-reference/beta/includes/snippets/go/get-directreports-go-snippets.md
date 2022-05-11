---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ced6a734b50a9dd4e84a972f4fd44285dbdf9dfa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().DirectReports().Get()


```