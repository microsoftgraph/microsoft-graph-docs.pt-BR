---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4987b229c4866b05ce29baeeac628ffc04e830e4fb918997bced7e8202c512a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329166"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.parentFolderId = "parentFolderId-value";
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders("{id}")
    .buildRequest()
    .patch(contactFolder);

```