---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13bfda0976ee067da0cf99716e7f779807342b7e35591b26faa80d8681310ca9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/allowedUsers/{userId}/$ref')
    .delete();

```