---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba4147b1b1e159bf8d4482dbbeb6506a3003bead4872ee72a6b4578dedc1d560
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/{id}')
    .version('beta')
    .get();

```