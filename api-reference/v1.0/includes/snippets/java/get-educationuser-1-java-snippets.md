---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85164a938fb25461a3cbb8e55dc70ef809c583e8eb5a76e8353cdc16aaf0908c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100255"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.education().me().user()
    .buildRequest()
    .get();

```