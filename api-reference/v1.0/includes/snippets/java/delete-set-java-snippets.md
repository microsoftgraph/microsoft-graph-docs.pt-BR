---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adbb292ae9314a02d57e6fcb9327224c8386a431
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().sets("8861b57a-c777-49e7-826f-47d6afecf80d")
    .buildRequest()
    .delete();

```