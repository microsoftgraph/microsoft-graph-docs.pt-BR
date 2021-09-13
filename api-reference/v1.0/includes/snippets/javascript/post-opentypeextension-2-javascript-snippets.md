---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e48f86e4dd7da7ffdee4986d1e5eb5935f331d8d85b85ef80ce996eb21b9726
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272904"
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