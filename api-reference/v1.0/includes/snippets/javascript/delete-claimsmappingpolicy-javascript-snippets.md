---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1564df822dcb546c94d6ea574a83854676c404e046bab66ee21b63c458d50ed8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/claimsMappingPolicies/{id}')
    .delete();

```