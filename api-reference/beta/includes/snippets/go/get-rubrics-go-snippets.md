---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32519ff5943714cda46209e8cc336db34dfb07a4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Me().Rubrics().Get(options)


```