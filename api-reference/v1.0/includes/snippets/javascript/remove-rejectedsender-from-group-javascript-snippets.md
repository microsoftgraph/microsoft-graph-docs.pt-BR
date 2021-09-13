---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 762996afbd3cfa9cf49313c5e7f68bf2c3a45307d83099dab80419b570b1fad3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/rejectedSenders/$ref')
    .delete();

```