---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e72a18ee4bb614db8f9abb3e6a93838a08ee1b33
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Delete()


```