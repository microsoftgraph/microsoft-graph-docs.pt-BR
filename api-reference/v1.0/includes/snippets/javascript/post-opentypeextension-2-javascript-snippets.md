---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da29a3df02ac02e6722d84e6bcb84f8e395a8570
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  '@odata.type': 'microsoft.graph.openTypeExtension',
  extensionName: 'Com.Contoso.Referral',
  companyName: 'Wingtip Toys',
  dealValue: 500050,
  expirationDate: '2015-12-03T10:00:00.000Z'
};

await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions')
    .post(extension);

```