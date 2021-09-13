---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aeff3d32aa0d565442298bf69b7ae8ffc07457d9c9ac26e5a80ac73e0c6e1a67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Groups["{group-id}"].Events["{event-id}"]
    .Request()
    .GetAsync();

```