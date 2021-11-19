---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95226cf2acaf408bf1d79901b912725163ccb198
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Delete(options)


```