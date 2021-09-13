---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5d16a3692dc09a7e49ec56dba388574d0ee6936f7ed8724a2bd72f613a49802
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .expand('userAttribute')
    .get();

```