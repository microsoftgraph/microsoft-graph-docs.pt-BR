---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c84bfc3a97b24511cbe4ff4a9683693dea2be61490216cc6506c5583eb704a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printerShare = await client.api('/print/shares/{printerShareId}')
    .select('id,displayName,capabilities')
    .get();

```