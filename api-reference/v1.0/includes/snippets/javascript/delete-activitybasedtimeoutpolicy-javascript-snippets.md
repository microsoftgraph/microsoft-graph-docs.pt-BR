---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7f344058d390b94a99ad246ac8a04024a93cffacf2961768ba6ea3a29b9c682
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .delete();

```