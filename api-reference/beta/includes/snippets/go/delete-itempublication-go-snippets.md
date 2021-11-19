---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c1d7a4b83c54a32b9ac06a101f2d1c5ddf1d4d5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093243"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPublicationId := "itemPublication-id"
graphClient.Me().Profile().PublicationsById(&itemPublicationId).Delete(options)


```