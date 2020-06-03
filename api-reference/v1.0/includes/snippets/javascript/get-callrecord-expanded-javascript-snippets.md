---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e366c84108a415b4e55cf66c98b18ea7ab7e04d4
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .expand('sessions($expand=segments)')
    .get();

```