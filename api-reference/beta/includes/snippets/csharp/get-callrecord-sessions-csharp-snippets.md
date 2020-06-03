---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c11f41d1633bee980a2f457410666b48ba26a64d
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{id}"].Sessions
    .Request()
    .GetAsync();

```