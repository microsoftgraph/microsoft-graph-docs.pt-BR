---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4de587a7a6f0bfbfed148e43ae0da60d6c628205
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325432"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

qnaId := "qna-id"
graphClient.Search().QnasById(&qnaId).Delete()


```