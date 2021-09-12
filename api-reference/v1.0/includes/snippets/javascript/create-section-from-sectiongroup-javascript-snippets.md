---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62b5b53ccb24adc887a774ce533552ad679b1700b40005bfb4b9dec3327a7ce3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216461"
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
    .post(onenoteSection);

```