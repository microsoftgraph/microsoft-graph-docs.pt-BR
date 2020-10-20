---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb0bf591b2591a0104e6ceee5b0451e9f1075c5f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings/{id}')
    .version('beta')
    .get();

```