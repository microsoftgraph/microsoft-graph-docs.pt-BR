---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 704cce82a1bfdcb96181b64bbb081aa719cabbea
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies/{id}')
    .get();

```