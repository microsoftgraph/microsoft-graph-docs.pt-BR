---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5b39a445e1d621532d67a5d5784514fd9e87b441b005745e12251b5b626317a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159562"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegrations = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .get();

```