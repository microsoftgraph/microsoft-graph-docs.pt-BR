---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05972973df40c9bfe9a409ef30cff69d7bff47cdf4d89d394448ce8fef413d4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .unfollow()
    .buildRequest()
    .post();

```