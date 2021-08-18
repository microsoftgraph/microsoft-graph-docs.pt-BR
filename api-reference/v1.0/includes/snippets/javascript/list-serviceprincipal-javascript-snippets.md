---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89c5818a859330c7f2b2c83ba0aee7d5181be5b83735824083492b0e80c07773
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .get();

```