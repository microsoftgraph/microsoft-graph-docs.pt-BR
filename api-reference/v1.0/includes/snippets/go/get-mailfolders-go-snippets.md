---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61284d5991f2e9cfcca6b98929317d298c641df6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091103"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().MailFolders().Get(options)


```