---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c41ffdfa37f8a8836d3727d14ac804321bb07a8
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pinnedMessages = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/pinnedMessages')
    .version('beta')
    .expand('message')
    .get();

```