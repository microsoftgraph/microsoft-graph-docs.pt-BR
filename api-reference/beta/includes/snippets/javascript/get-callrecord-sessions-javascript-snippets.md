---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 089d02434c902e712646e0f99daf042e2cbbf2b4b9beb36f959022924e13ffa1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .get();

```