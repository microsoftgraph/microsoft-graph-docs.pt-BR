---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c11f41d1633bee980a2f457410666b48ba26a64d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473880"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{id}"].Sessions
    .Request()
    .GetAsync();

```