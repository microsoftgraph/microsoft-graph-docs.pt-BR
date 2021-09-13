---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 065c5caa8c3ce57bfff6a01cfcfc2e5743cb6eb0466854f9f775fc727d00d4d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudits = await graphClient.AuditLogs.DirectoryAudits
    .Request()
    .GetAsync();

```