---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04263fe632ecbc1cf11dec3073fde3d58219e98f1c3c7758bd8cac276b679c72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099384"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().educationalActivities("{id}")
    .buildRequest()
    .delete();

```