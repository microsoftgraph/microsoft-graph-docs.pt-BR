---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8c8f45a5ac48514f3a3dad610b49e3dff13f6ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967106"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .clear()
    .buildRequest()
    .post();

```