---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bff7547f658bc5e6f80c6abaed194763359a36bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974131"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().contactFolders("{id}")
    .buildRequest()
    .delete();

```