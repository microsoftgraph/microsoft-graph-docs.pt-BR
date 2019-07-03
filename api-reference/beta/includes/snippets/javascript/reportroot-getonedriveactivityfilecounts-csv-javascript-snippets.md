---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8011b988e8440c14c312dd0533053f9e388c9d47
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```