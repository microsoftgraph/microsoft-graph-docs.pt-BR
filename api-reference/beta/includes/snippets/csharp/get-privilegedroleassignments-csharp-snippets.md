---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e13366021151d86824b311afadc05b4b676321
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .Filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
    .GetAsync();

```