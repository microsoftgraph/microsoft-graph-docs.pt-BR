---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83e72b74dfa15b653deec9dd21cd0b799e6d7a7c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978538"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .delete();

```