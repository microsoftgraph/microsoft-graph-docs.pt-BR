---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8badfdff47c734a20b212ff910469f1fcaae29f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/archive')
    .post();

```