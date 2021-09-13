---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 608d1036969aafe56f79902fc47de840346b1239093f7708b0be993f4523d55c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .get();

```