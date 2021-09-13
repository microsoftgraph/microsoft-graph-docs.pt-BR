---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed800ef5ea33c0b2e00e13595cceda1390603de3461049c2d71331e7fb953652
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deletedItems/{object-id}')
    .delete();

```