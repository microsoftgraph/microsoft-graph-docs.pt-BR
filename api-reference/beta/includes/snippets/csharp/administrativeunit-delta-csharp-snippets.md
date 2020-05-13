---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35cd74713352c3d803407d90248af0eeaeebbd2b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Administrativeunits
    .Delta()
    .Request()
    .GetAsync();

```