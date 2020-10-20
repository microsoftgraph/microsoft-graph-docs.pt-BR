---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28782297c2e9a719f5cbc31b7f2d9f129eb6450e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true,')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```