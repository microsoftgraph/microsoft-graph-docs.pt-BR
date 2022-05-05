---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8dde2c1b777affe00b226937cd13d95cfe6e43a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("root").lists("Documents").items("2").documentSetVersions("1")
    .restore()
    .buildRequest()
    .post();

```