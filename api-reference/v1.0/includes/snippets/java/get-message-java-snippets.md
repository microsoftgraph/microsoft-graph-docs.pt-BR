---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3689c4cbe8daa285efab04af9eaca81a4c836eaefc23899c51973fa6338997e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhMGAAA=")
    .buildRequest()
    .get();

```