---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2813245a0f44cafb13a54ef0b2c32e300e7c2c0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083641"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().WebAccounts().Get(options)


```