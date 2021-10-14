---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbc9ab4e5319bfd2e7005aee14ccbc3edcc5af0fbc66daeb1291e2a7b89b6ce0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/unarchive')
    .version('beta')
    .post();

```