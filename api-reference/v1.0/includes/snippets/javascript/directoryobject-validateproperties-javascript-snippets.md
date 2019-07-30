---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8ce36e825a5cc2f665a4dc32ef781fe33658ad0
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  entityType: "Group",
  displayName: "Myprefix_test_mysuffix",
  mailNickname: "Myprefix_test_mysuffix",
  onBehalfOfUserId: "onBehalfOfUserId-value"
};

let res = await client.api('/directoryObjects/validateProperties')
    .post(validateProperties);

```