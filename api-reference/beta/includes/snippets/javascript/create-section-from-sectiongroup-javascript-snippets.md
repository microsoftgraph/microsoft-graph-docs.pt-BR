---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b312bac888fe2565d1b71fc9bf80b2bef84d77ce9e44caefe519ae82c448027
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: 'Section name'
};

await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .post(onenoteSection);

```