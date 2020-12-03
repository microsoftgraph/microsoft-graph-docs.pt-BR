---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 600429988d8e25f9c9dd1652a83a4b5503afadaa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062"].Members["ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk="]
    .Request()
    .DeleteAsync();

```