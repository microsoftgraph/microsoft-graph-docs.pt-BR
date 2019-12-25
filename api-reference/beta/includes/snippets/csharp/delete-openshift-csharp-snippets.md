---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 799e6db2f0042b56e40f7cae7bce37acf28f0c7c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.OpenShifts
    .Request()
    .DeleteAsync();

```