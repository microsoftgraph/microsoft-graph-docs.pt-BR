---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16168b07fdf16249dc4e121f3a3d0dd6f9880ac4a19d4c60885a24fa267192c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/sites/{site-id}/lists')
    .version('beta')
    .get();

```