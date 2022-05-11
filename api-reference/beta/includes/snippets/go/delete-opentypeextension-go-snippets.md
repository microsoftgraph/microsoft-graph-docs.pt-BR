---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b08abec501973a4a92d20d7ec6718fbff06a6c75
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Delete()


```