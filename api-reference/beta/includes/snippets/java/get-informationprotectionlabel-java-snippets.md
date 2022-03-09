---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 726b3af94d376bddb3b75be6948a7e5722dcf7b471a3a652700d6ee153a055e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213586"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InformationProtectionLabel informationProtectionLabel = graphClient.me().informationProtection().policy().labels("{id}")
    .buildRequest()
    .get();

```