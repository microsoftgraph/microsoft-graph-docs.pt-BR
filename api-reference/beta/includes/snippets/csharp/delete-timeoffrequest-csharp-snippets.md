---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9be327af3f1a3197c2520862b3ebbac0d8f3c1d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.TimeOffRequests
    .Request()
    .DeleteAsync();

```