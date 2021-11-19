---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c5a9f8c0ab9cbac469c3c78dc24a57e85f37613
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103170"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Onenote().SectionGroups().Get(options)


```