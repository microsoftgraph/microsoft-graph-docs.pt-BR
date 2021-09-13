---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f4a943bc6a4547e467e1377bfc72bd837ae93a3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getApplicableContentTypesForList = await client.api('/sites/{siteId}/getApplicableContentTypesForList(listId='listId')')
    .get();

```