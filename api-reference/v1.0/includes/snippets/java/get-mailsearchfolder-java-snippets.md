---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87c5d91d96138636a381832b225a7da1f73a964e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983095"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzN")
    .buildRequest()
    .get();

```