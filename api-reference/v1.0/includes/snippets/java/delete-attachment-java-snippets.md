---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 894b9af9cfeff5f3496bc627b6493473c774b1b78ec7611edcff5b492827e953
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329491"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}").attachments("{id}")
    .buildRequest()
    .delete();

```