---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60a5b82940fa7908463bf62797be31f21f28c8190ce1d62b6dcb5842a5de4cd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158220"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderCollectionPage mailFolders = graphClient.me().mailFolders()
    .buildRequest()
    .get();

```