---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9d19172489c7bec313b079b18c6e587a135db14123cbede4c48e5acbb7ad2de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .delete();

```