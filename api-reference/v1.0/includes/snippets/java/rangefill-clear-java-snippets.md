---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 115ea0e42220a3e9e6ebe88e5ff3fb5fcb1ac22abe1da52249481dd0784388b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100229"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .clear()
    .buildRequest()
    .post();

```