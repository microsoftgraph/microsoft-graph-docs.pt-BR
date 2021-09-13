---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99a3b1bd855138f5b72eee6b8d2f883934cee7fb12c480c1b71c99338a0b5bd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
contact.givenName = "Pavel";
contact.surname = "Bansky";
LinkedList<EmailAddress> emailAddressesList = new LinkedList<EmailAddress>();
EmailAddress emailAddresses = new EmailAddress();
emailAddresses.address = "pavelb@fabrikam.onmicrosoft.com";
emailAddresses.name = "Pavel Bansky";
emailAddressesList.add(emailAddresses);
contact.emailAddresses = emailAddressesList;
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 732 555 0102");
contact.businessPhones = businessPhonesList;

graphClient.me().contacts()
    .buildRequest()
    .post(contact);

```