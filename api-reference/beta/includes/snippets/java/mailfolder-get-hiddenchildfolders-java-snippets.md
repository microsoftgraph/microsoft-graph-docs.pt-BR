---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc5f3ca3d4dd120466a6454a8a4dfeee14c6a395
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665246"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("includeHiddenFolders", "true"));

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("AAMkAGVmMDEzM").childFolders()
    .buildRequest( requestOptions )
    .get();

```