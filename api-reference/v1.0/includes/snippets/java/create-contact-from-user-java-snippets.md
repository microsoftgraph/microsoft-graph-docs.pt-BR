---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70f4a12b2581a804fef0131bd6565e4aa3d81784
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978887"
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