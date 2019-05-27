---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cffef970a55583a79202d9b31a5d0d75c8b535dd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["{class-id}"].Teachers
    .Request()
    .GetAsync();

```