---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afbdbb658fa38ceb2eeaf5fa71d5969ba94f7d91
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .version('beta')
    .post();

```