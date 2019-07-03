---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c18dfdd84198a9acfa5935febe670792f90a8ecf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)')
    .get();

```