---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f87b54787a803d86d143af0e35071a5c53be911a
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .get();

```