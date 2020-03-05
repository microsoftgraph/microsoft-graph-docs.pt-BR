---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c01efcd66a138bc47931940b98a54aece95042c8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .get();

```