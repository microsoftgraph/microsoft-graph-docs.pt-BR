---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65d4403cd034342f7e9e1bd544f7272c95295d96
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries')
    .version('beta')
    .get();

```