---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49ceee179c34663c5740cac3d085b589fcbdcc93b663ab0b7810a45fb48a4921
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Education.Me.User
    .Request()
    .GetAsync();

```