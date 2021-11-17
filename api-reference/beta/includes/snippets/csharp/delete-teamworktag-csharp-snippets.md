---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abcb3fa5f2cef6838274e3ffafb8318a97afca7e1f819c5270c3c2bb1a8c50e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"]
    .Request()
    .DeleteAsync();

```