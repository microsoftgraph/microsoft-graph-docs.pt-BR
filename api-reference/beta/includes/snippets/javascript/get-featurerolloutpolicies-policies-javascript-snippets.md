---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60ce931073cb063a55d14e864e8fbc7d46bfc5455d7e6b793aa81d0e418d6731
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicies = await client.api('/policies/featureRolloutPolicies')
    .version('beta')
    .get();

```