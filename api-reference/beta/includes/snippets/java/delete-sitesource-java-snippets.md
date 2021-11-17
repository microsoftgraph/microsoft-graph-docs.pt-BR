---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb74cf5bd84cd6f1d7aec027b171fb5a6d794603fb7ebd7f8a923ecae503581e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157233"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").siteSources("38304445-3741-3333-4233-344238454333")
    .buildRequest()
    .delete();

```