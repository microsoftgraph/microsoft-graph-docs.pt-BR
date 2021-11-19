---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acfeaa09fb3c0720ae8fa42073073b7c89436cb6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086274"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().CreatedObjects().Get(options)


```