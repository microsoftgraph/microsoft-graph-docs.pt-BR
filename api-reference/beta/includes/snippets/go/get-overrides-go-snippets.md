---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91c1f683c0a785eabe730b527bd45b83eae38175
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085362"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InferenceClassification().Overrides().Get(options)


```