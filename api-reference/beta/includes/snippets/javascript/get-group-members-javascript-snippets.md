---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e313d25365db89d9341133b0edd534e629641fd653fe0ebc91f467150296261d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```