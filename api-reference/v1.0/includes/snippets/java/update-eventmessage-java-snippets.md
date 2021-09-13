---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57ab2ccde33483fb34309acf62c33d61ea41d7eb3551c71d9b73d795db3e0687
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899317"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = true;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```