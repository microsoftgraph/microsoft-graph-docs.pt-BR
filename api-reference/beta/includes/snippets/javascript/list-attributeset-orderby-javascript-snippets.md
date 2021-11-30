---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 559188a82889e00070428808f0dcf516fa7984b9
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attributeSets = await client.api('/directory/attributeSets')
    .version('beta')
    .orderby('id')
    .get();

```