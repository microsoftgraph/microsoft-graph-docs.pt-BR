---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24d6a8f82650cf5bcde10227d7f6385c8a562f05bfa369871f7e4563072d1c6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.Groups["{group-id}"].GroupLifecyclePolicies
    .Request()
    .GetAsync();

```