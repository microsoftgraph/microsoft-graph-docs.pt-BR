---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0b0ebdd069aee8a8f15fa720854395fc41652b429a9b3cb81110827ffb0edfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```