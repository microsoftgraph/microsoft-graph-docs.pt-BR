---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82d43f8cc80d0cbc044039323e46beaf6d3b0a2d3bec9195f5c9043d80606c64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().seriesAxis().format().line()
    .clear()
    .buildRequest()
    .post();

```