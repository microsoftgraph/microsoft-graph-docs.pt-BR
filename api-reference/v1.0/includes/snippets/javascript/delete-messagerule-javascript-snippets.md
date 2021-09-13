---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d54e4d112be670ec3b560fe183dbbb9af09f6b3abc732a35cda2b5e53dd0f88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=')
    .delete();

```