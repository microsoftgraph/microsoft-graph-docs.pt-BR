---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2513b037b27050cbf97d3adf95f06aa977a61ee6eb0853e7a324b4ace7b899b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfiles = await graphClient.Security.SecureScoreControlProfiles
    .Request()
    .GetAsync();

```