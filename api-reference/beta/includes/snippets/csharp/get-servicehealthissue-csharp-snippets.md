---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b0a97ec25ca9b30ef00b2a699647c00091a6ee9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealthIssue = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .Request()
    .GetAsync();

```