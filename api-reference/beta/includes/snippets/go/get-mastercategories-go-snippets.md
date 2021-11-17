---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3b5bcac3bc9b22f421bdec7c4ad70bddf145c79
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004636"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Outlook().MasterCategories().Get(options)


```