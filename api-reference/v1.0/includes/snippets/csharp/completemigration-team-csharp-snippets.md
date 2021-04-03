---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebba3b1955a8888b7f24e240682f91a449a76caf
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```