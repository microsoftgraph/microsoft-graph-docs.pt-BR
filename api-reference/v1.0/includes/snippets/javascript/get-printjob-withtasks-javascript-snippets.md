---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6561bd1908ea61e16729c844e3bb12a30a3b0c976f9bb7729c733b0353213c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/{printerId}/jobs/{printJobId}')
    .expand('tasks')
    .get();

```