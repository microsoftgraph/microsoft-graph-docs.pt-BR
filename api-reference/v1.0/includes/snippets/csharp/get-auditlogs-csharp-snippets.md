---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a185b0f12682b42214ed66b544c1b33fbd26b9da33296684f1cc940bac367c03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditLogRoot = await graphClient.AuditLogs
    .Request()
    .GetAsync();

```