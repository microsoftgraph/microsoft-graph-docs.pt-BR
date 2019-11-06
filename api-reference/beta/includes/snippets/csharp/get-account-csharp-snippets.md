---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98545914a0c0bfc108a1ad69437dfce07749548a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var account = await graphClient.Me.Profile.Account
    .Request()
    .GetAsync();

```