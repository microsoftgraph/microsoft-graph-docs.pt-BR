---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed4a15289368d3400ecaeb9e8f0b47cdc48f737d85f2d4c4cf7c676117ed97a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.Policies["{conditionalAccessPolicy-id}"]
    .Request()
    .DeleteAsync();

```