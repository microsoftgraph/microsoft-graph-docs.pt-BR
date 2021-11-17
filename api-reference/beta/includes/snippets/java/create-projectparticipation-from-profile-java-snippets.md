---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c653fe27848d32649cbf7511e63b5a1eb6099186c97635fb254f4b5899dfb4bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217376"
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