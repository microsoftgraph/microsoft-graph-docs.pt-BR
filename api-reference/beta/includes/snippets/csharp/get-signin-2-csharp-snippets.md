---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa1f4d787169e5f37340ca755e6f0f75dc34d61f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIn = await graphClient.AuditLogs.SignIns["{id}"]
    .Request()
    .GetAsync();

```