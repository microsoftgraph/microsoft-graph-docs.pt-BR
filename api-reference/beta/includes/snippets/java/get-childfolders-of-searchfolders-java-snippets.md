---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20f3f73482f6451da0a6f08a2ee2c682975f81686e903e21e97c6e3b847fb016
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("searchfolders").childFolders()
    .buildRequest()
    .get();

```