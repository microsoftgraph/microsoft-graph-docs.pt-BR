---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27953aa00c1e405b6b3900d654f693f1d0148aa7be0409d5970b848ae6e4eba4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/me/schools')
    .version('beta')
    .get();

```