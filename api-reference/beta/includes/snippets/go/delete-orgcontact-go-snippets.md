---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b41791db5b725b0401d3cbe0cbc024c4cb2d52c4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).Delete(options)


```