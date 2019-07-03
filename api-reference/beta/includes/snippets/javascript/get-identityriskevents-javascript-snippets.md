---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0af8b1afaf83ff606a2ff2331aff94305afa5d24
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477820"
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