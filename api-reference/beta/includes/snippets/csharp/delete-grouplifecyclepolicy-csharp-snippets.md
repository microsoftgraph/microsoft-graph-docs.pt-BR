---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17357684c8299af8c6db0bea1aa7e6cb4c31e96daf9eb28d2f051f1c10bdf98b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupLifecyclePolicies["{groupLifecyclePolicy-id}"]
    .Request()
    .DeleteAsync();

```