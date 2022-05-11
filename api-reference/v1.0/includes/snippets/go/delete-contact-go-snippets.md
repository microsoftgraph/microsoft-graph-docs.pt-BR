---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3efcb05e9641dd1e658f6732a8590678e4a809e1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323182"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Delete()


```