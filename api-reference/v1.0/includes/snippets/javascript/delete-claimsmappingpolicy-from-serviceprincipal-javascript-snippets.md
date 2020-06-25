---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01fc0d9284d96bd3ec8e5f4ee3cb7df80f5dc915
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref')
    .delete();

```