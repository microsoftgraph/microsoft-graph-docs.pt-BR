---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8dbc4faf7c1414c364cd5e2a952acf898a5801a8315e00b2dc62934a521c2cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let application = await client.api('/applications/{id}')
    .get();

```