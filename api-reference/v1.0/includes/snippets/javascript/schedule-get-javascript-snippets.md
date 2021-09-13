---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3da2ccc794fcd0b1c5181aebd1f8d9555724ef764bb8c6e7a1b59627cdcbfc76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedule = await client.api('/teams/{teamId}/schedule')
    .get();

```