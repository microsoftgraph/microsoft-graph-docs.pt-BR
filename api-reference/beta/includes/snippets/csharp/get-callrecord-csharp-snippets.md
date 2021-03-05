---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5db6923a49454290f96e123da14ce81d28747ae5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .GetAsync();

```