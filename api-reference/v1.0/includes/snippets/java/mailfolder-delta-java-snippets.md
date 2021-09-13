---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97c909e6d0a7cc4b88ced368b034c918228d66421d5bdb5fd4ec8465a2726a7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217069"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderDeltaCollectionPage delta = graphClient.me().mailFolders()
    .delta()
    .buildRequest()
    .get();

```