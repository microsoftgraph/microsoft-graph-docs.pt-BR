---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9e553fac8299699d1ec6d52f30724549021a5bb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).Get(options)


```