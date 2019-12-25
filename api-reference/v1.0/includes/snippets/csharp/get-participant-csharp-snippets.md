---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6332fae7397b6dbb1a478113cde8bbe27d4a74cc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participant = await graphClient.Communications.Calls["7531d31f-d10d-44de-802f-c569dbca451c"].Participants["7e1b4346-85a6-4bdd-abe3-d11c5d420efe"]
    .Request()
    .GetAsync();

```