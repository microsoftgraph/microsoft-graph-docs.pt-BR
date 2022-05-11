---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9efc30e6e3841e600d955e547d8b2b8f38a53773
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322508"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Close(case-id).Post()


```