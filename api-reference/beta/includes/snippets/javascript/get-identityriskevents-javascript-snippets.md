---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0af8b1afaf83ff606a2ff2331aff94305afa5d24
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityRiskEvents')
    .version('beta')
    .get();

```