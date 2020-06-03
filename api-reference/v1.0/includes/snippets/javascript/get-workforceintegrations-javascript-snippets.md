---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8125f0715fc19f31dbb78b2cd5a1d5ed8017d9bb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teamwork/workforceIntegrations')
    .get();

```