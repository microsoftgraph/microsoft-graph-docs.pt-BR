---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2634708bb0071fd811394e1e79c35890ef8890d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile
    .Request()
    .DeleteAsync();

```