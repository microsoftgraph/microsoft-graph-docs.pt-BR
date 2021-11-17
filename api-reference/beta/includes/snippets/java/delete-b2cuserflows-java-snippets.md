---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f022e3185ce242044c26f88c7731723c16f559257151b71504264d59bf72f170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898855"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .delete();

```