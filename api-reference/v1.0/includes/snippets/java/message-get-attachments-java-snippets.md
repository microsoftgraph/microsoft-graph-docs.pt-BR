---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 558f05029b98369630253d10b27489683ceb54f1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462018"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .get();

```