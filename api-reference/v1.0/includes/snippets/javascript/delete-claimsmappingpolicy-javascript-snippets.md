---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 806ee7beebd53dc489de0ef7d538c74410663859
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/claimsMappingPolicies/{id}')
    .delete();

```