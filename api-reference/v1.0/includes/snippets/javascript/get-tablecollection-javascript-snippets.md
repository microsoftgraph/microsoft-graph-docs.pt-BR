---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fad18d05eb54efd0dfa2e4ab46c120f6bbe942c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables')
    .get();

```