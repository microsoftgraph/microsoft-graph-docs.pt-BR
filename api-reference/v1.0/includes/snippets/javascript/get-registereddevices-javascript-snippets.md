---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5aa7e87dae7ac7a2449ad08bc7cab97ad1dc1d3d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/registeredDevices')
    .get();

```