---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b907a3db35b1fbf5ed08672617b69e64123dcb24ca201f0cc0145155e848a3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let emails = await client.api('/me/profile/emails')
    .version('beta')
    .get();

```