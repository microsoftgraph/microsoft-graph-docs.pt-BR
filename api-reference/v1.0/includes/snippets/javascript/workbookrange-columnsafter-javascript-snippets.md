---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2c2e158ec83d00efe7fe02a62f6c2ee3aee4839
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)')
    .get();

```