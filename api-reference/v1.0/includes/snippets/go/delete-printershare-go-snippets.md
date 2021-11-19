---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04dab2ba5f04dbcfb0ceea5865c619228be2c821
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099135"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Delete(options)


```