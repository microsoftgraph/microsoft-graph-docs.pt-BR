---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fad18d05eb54efd0dfa2e4ab46c120f6bbe942c8
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables')
    .get();

```