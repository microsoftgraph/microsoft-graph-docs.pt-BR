---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e79d1878a43856f3671ed26054f5b39c2e1406e11c8314782cf1a579dfbcc04e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376556"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("{id}")
    .buildRequest()
    .delete();

```