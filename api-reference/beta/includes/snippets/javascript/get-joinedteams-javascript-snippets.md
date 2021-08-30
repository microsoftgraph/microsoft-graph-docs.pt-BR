---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc284c4f134963a933bd20c89a95fd16857743a6e6386a700217955ee251c954
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let joinedTeams = await client.api('/me/joinedTeams')
    .version('beta')
    .get();

```