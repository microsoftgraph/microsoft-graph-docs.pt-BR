---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57780972556a21a5e406c4e55bcd412df9efe30b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["B2C_1_testuserflow"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```