---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0176fb44d695c251c7aaa8e7c6a05b9029cb215dce001f490105392c7bddbca3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive')
    .version('beta')
    .post();

```