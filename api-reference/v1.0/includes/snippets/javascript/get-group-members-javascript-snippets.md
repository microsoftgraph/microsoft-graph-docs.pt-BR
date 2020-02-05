---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 247493fba342f37d38a991bfd5478d5e88b83f69
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .get();

```