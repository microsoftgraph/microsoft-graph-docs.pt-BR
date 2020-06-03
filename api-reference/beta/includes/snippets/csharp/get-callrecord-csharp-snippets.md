---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5db6923a49454290f96e123da14ce81d28747ae5
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .GetAsync();

```