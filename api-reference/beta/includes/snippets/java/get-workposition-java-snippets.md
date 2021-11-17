---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24b664e7f5246c068c9323c20ff59d651c3569fdaaaa19ebd609bd343e5a1206
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = graphClient.me().profile().positions("{id}")
    .buildRequest()
    .get();

```