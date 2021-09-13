---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47160d985e1826058fb7437c84099a2ff03df41aa49f9df6ff38d6c78950a4d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275722"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("3856fd6f-36e2-4152-97c9-76070d19f730")
    .buildRequest()
    .delete();

```