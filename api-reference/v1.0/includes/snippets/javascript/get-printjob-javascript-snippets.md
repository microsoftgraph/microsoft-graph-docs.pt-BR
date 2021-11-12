---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8a6bd903072d9be9d9109360c71126dec8908a6cc0e913a5a0135b7cbf7b5b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/{printerId}/jobs/{printJobId}')
    .get();

```