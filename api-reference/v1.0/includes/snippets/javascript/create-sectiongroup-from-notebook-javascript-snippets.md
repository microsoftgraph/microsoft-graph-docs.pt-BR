---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96f10afbdc73c0b264e4978eae18557eee48fbb698a3b5d0a58d918dc1cf3834
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .post(sectionGroup);

```