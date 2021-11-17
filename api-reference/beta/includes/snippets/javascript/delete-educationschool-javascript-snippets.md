---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17a73dae08bd531b39f5611efe0eaaf735fb668783cec9acab2f48bd8dd24513
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10002')
    .version('beta')
    .delete();

```