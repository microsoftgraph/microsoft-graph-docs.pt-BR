---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5994be4c43b2c66ea3a84e5ea50cde9eba5c819a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

await graphClient.Communications.Calls["{id}"]
    .SubscribeToTone(clientContext)
    .Request()
    .PostAsync();

```