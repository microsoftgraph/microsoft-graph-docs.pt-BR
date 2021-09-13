---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3fbca9c58b704d3d9c0b40f6dbc708a0658c2a39ac6b83a6dcc15f89588ef64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407071"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments("City")
    .buildRequest()
    .delete();

```