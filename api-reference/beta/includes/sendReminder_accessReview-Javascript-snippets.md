---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4b3dae19d10a1e68287fc07fef0e4ce09477afa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder')
    .version('beta')
    .post();

```