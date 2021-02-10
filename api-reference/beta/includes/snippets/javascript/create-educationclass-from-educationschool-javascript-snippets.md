---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4ab7b63be36c31946206554f1c78d2e309a56e6
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{id}/teachers/14012')
    .version('beta')
    .delete();

```