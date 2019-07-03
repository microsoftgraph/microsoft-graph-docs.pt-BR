---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebfca6a4001f3be672ee174065d6395f59997c3f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .get();

```