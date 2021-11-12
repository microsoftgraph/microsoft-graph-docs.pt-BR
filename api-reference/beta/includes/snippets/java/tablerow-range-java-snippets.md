---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e8147545c66dfa4361d6c91bf5814b301894c3c0ff5347bcddfdeb37b6492ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .range()
    .buildRequest()
    .get();

```