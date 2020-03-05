---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbc72fa0a3e4f766712487da22d72778796796cd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992906"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{id}"]
    .Request()
    .DeleteAsync();

```