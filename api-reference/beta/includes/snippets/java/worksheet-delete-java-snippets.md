---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e06b1fe5b503a32e3e96485e6bb2691b7917cf15
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979873"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .delete();

```