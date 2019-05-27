---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df667e3e22f0fad71a18fa72d25385296fc98071
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{class-id}"]
    .Request()
    .DeleteAsync();

```