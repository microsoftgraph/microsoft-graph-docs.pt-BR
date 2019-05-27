---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1eceaeeb8212ee05cbb8c73b046820cf37cc8f38
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/start')
    .version('beta')
    .post();

```