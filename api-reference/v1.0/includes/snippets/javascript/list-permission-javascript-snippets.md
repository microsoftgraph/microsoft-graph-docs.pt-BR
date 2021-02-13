---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbed28be705bb478c3349ab834e907d0aed5e762
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176820"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions')
    .get();

```