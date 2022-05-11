---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86ef20cb35eb81bae64da335daab12d7b2964088
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceUpdateMessageId := "serviceUpdateMessage-id"
result, err := graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).Get()


```