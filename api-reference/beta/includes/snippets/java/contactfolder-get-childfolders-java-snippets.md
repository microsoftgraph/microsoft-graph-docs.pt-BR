---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b53cfd43690483bca891dfb4486fffa52f85698a6bb2f396395c31431ed08b7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273558"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolderCollectionPage childFolders = graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .get();

```