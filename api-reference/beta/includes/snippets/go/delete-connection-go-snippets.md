---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3770883f319e06beec576d82503d9176fbe9c0ab
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101169"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Delete(options)


```