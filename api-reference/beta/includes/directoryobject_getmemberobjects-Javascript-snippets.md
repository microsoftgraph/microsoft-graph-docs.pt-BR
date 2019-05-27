---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33f10e9e477e0b44f5612c3b22c72e14cba1c0a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberObjects')
    .version('beta')
    .post(String);

```