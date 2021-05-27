---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f69186936bcf8043eff233bc8616538a492a021e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().identityProviders("{id}")
    .buildRequest()
    .delete();

```