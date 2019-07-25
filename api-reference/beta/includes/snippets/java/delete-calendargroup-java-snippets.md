---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2333d5b82aff2ee7032a4400ba43519be95bf219
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864974"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .delete();

```