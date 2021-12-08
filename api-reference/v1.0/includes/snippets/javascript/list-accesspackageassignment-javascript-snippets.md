---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40ce2fdc2e4706bd91187d2619500a7ee56cf718
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/identityGovernance/entitlementManagement/assignments')
    .get();

```