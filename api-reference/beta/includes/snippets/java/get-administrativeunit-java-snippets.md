---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afedd17b4fa83aeb6424c94f9eff879de6a76f7c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962622"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.administrativeUnits("{id}")
    .buildRequest()
    .get();

```