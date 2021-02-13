---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3df79eb3328504df7db2b267bb84e4be5c3b184
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .delete();

```