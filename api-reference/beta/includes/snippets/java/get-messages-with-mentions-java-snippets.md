---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 403dedef55ed3f28a3c9c662913194f4f509db3c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176987"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .filter("MentionsPreview/IsMentioned eq true")
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```