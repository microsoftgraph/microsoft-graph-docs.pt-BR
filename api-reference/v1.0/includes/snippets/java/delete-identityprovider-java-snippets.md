---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f69186936bcf8043eff233bc8616538a492a021e
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().identityProviders("{id}")
    .buildRequest()
    .delete();

```