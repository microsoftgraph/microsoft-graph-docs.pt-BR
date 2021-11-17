---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0ae8b023aa8004867ee11de1deb844ff23152c3d57c7a3c91a1733b5fbc215e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.administrativeUnits("{id}")
    .buildRequest()
    .delete();

```