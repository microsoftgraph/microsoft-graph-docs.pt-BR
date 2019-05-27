---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53e711ba87e75573e4e32226473b617a5b8889fd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserDetail')
    .version('beta')
    .get();

```