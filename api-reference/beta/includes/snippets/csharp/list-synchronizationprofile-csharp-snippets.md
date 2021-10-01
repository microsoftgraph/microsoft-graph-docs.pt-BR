---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6402e560567792863f5de205c77844eb003b5f70739ca3ae01f489f5d87fb8e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationProfiles = await graphClient.Education.SynchronizationProfiles
    .Request()
    .GetAsync();

```