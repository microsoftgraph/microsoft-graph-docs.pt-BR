---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ef6982083385a1a1ec7032b5cb1bd559027fde5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().People().Get(options)


```