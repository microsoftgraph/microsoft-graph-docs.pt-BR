---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e60a5916290d6c1feb0a8fe6a8a1d46cfb76402d0be6495edaa2f5baff9949f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407105"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADYAAAImV_lAAA=")
    .buildRequest()
    .get();

```