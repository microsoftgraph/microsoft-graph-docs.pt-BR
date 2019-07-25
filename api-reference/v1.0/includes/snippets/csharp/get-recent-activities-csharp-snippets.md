---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae9d7d2a4bacaf423a64e34aec181c14510aa0a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities
    .Recent()
    .Request()
    .GetAsync();

```