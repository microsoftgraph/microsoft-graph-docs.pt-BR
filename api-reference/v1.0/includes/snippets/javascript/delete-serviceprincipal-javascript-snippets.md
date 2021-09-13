---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95ebd93553fea009616d90de70c1de881f27db4833e73a8696fdb7510058e789
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}')
    .delete();

```