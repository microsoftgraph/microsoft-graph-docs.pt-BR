---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3d6f99357b6cde4723b412925cbd1da055070d2a5bfb075701a467fbec635f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214744"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.planner().rosters("5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38")
    .buildRequest()
    .delete();

```