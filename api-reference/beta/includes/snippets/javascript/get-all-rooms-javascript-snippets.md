---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85a49dd92f98ed4d80398ac0312a8a34d0e11528
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/microsoft.graph.room')
    .version('beta')
    .get();

```