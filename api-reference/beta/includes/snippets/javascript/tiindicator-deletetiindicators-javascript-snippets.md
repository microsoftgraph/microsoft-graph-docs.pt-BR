---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85c353ad097a11421a05a43710b64fa56168fb782382900272d4a7fc7d50bf49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resultInfo = {
  value: [
    'id-value1',
    'id-value2'
  ]
};

await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(resultInfo);

```