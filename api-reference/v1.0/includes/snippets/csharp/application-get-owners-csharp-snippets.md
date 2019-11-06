---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d16f0492ac0fd46779bb22045a2f254c6baaa1fa
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Applications["{id}"].Owners
    .Request()
    .GetAsync();

```