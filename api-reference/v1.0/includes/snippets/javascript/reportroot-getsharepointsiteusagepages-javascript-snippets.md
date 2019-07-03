---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52a4dfef3b26bbcd4f471c25aacafdb96200e1eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsagePages(period='D7')')
    .get();

```