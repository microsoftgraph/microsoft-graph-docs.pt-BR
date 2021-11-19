---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8c9413b33e9a777d832b0b2bc4d728fcbb9cc57
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().Windows().Updates().Deployments().Get(options)


```