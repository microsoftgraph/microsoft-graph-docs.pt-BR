---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad27cf72f0ff2e30d5bf0d5b2498f22630db8f9337310707f2367fad1f600dd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10002")
    .buildRequest()
    .delete();

```