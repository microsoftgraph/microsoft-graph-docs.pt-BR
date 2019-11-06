---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcb2eb5b2d80604694f7d8321907ade6799f69a2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns/{id}')
    .version('beta')
    .get();

```