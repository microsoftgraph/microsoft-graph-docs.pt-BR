---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6efe47b0945060e52caf933f1a5e1a0b6532c8fd70c41905de185e8461ac84ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let skills = await client.api('/me/profile/skills')
    .version('beta')
    .get();

```