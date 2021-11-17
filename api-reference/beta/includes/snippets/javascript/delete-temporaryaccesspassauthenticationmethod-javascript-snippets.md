---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23ab36e41caef49428c502efd38d046c8d66da1d217cd76fa46a4d7c6dafade4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}')
    .version('beta')
    .delete();

```