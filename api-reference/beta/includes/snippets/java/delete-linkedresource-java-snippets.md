---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b5500fcb5ac36796b25f3a9d3371350f2560cac5092743dd61b8d569af20a4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160181"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources("f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9")
    .buildRequest()
    .delete();

```