---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd44c232c1ab0f25f8c4acab45fb494a04a35f07
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsTab = await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d')
    .expand('teamsApp')
    .get();

```