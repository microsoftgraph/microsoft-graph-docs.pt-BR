---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 829ee9f5f9041246af2ebc3acdf17560993672616b971108d1b2e72d93edfab7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.GroupLifecyclePolicies
    .Request()
    .GetAsync();

```