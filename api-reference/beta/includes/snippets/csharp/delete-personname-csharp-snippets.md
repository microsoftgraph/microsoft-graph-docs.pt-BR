---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acd21915ceb0ef45c6543c8890af80465c826964981a298b2d5a2dc053cf4922
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .DeleteAsync();

```