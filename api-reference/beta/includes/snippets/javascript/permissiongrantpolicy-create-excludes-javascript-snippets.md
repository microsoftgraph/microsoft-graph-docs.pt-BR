---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a09f2efdbced653eb099547ca2602e535488289c8ef04c7a1a0061b2b962917
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: 'delegated',
  resourceApplication: '00000003-0000-0000-c000-000000000000'
};

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes')
    .version('beta')
    .post(permissionGrantConditionSet);

```