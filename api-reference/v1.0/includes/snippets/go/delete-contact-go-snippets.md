---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7de1ec266e78fc47d7cc21e0319fa33b603763e8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285925"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Delete(nil)


```