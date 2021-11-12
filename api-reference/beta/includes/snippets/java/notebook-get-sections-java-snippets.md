---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f8bc6cf47f446f5739ecf435c4d66c1011b92c2040518ff7ee1f1fe4577d95b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSectionCollectionPage sections = graphClient.me().onenote().notebooks("{id}").sections()
    .buildRequest()
    .get();

```