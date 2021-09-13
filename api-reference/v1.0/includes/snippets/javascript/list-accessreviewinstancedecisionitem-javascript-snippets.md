---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5515e5e35d0c6b45db51d67dbf58b545ce7518194c08d6bac4f1f66899e1e168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances/8d035c9d-798d-47fa-beb4-f986a4b8126f/decisions')
    .get();

```