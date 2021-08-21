---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62d32b02497f9dcade6c4124bddaf35b797b6d0862e4a96480c0567f916ef853
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval
    .Request()
    .GetAsync();

```