---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2817d942a6b164cfab95caae9caaff979d06de6f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{idOrUserPrincipalName}/drive')
    .get();

```