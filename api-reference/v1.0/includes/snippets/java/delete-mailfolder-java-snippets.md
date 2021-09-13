---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1480c14383c1f66bd74ad4879931c594880f4ffbb16906dd796d4c6c65bf1c85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().mailFolders("{id}")
    .buildRequest()
    .delete();

```