---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2348a8ce55e97e313bbaa3e729f250a4938d1065
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = new ProjectParticipation();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Branding");
projectParticipation.categories = categoriesList;
CompanyDetail client = new CompanyDetail();
client.displayName = "Contoso Ltd.";
client.department = "Corporate Marketing";
client.webUrl = "https://www.contoso.com";
projectParticipation.client = client;
projectParticipation.displayName = "Contoso Re-branding Project";
PositionDetail detail = new PositionDetail();
CompanyDetail company = new CompanyDetail();
company.displayName = "Adventureworks Inc.";
company.department = "Consulting";
company.webUrl = "https://adventureworks.com";
detail.company = company;
detail.description = "Rebranding of Contoso Ltd.";
detail.jobTitle = "Lead PM Rebranding";
detail.role = "project management";
detail.summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization.";
projectParticipation.detail = detail;

graphClient.me().profile().projects()
    .buildRequest()
    .post(projectParticipation);

```