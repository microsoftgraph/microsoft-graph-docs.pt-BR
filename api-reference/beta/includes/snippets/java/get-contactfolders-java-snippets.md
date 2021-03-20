---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abbf4e81ed359ec2cb7f6672876d07b3a4a35eed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973433"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolderCollectionPage contactFolders = graphClient.me().contactFolders()
    .buildRequest()
    .get();

```