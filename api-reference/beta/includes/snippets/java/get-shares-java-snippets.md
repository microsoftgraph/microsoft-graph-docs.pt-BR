---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71fee77eff83b5043818f6e960c7e73c427e28a6baa68ba54f59c096963d6fca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328022"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShareCollectionPage shares = graphClient.print().shares()
    .buildRequest()
    .get();

```