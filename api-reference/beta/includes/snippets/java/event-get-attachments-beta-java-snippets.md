---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e93ec682dbfce6942d22f3b0e2c9692967eecb2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978177"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.me().events("{id}").attachments()
    .buildRequest()
    .get();

```