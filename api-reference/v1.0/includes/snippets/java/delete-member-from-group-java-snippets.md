---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0555dd97a8db18e3b36062487c11455cd5e9280
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890783"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").members("{id}").reference()
    .buildRequest()
    .delete();

```