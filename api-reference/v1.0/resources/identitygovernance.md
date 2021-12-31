---
title: Tipo de recurso identityGovernance
description: O singleton para conter recursos de governança de identidade.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: be8bb2f562b05892f972431fd32db72b29af305a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649680"
---
# <a name="identitygovernance-resource-type"></a>Tipo de recurso identityGovernance

Namespace: microsoft.graph

O singleton de governança de identidade é o contêiner para os seguintes recursos Azure Active Directory de governança de identidade que são expostos por meio dos seguintes recursos e APIs:

+ [Avaliações do Access](accessreviewsv2-overview.md)
+ [Gerenciamento de direitos](entitlementmanagement-overview.md)
+ [Consentimento do aplicativo](consentrequests-overview.md)
+ [Termos de uso](agreement.md)

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessReviews|[accessReviewSet](accessreviewset.md)| Contêiner para os recursos base que expõem a API e os recursos de críticas de acesso. Atualmente, expõe apenas o recurso [de definições.](accessreviewscheduledefinition.md)|
|appConsent|[appConsent](appconsentapprovalroute.md)| Contêiner para recursos básicos que expõem a API e os recursos de solicitação de consentimento do aplicativo. Atualmente, expõe apenas o [recurso appConsentRequests.](appconsentrequest.md)|
|entitlementManagement|[entitlementManagement](entitlementmanagement.md)| Contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)e [entitlementManagementSettings](entitlementmanagementsettings.md).|
|termsOfUse|[termsOfUseContainer](termsofusecontainer.md)| Contêiner para os recursos que expõem os termos de uso api e seus recursos, incluindo [contratos](agreement.md) e [agreementAcceptances](agreementacceptance.md). |

