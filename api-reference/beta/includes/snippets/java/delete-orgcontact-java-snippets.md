---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76f6f41f8c4d74747f3514bfec75613b456b2a4e2d18ea6cdd9c12a31308bafd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100046"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.contacts("{id}")
    .buildRequest()
    .delete();

```