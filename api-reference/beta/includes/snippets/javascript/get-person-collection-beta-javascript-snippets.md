---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4f4cd9109d126e3b4912ab630da6b1dd82da59d72fbd36296a0dad66849edfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let people = await client.api('/me/people')
    .version('beta')
    .get();

```