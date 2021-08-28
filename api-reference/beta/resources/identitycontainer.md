---
title: tipo de recurso identityContainer
description: Representa o ponto de entrada para diferentes recursos em Identidades Externas tanto para locatários do Azure Active Directory (Microsoft Azure AD) quanto para locatários do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 44c11b4e2280a38f243898a0e5b19dd5a63a1440
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668078"
---
# <a name="identitycontainer-resource-type"></a>tipo de recurso identityContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o ponto de entrada para diferentes recursos em [Identidades Externas](/azure/active-directory/external-identities/) tanto para locatários do Azure Active Directory (Azure AD) quanto para locatários do Azure AD B2C.

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|apiConnectors|Coleção [identityApiConnector](identityApiConnector.md)|Representa o ponto de entrada para conectores de API.|
|b2cUserFlows|Coleção [b2cIdentityUserFlow](b2cIdentityUserFlow.md)|Representa o ponto de entrada para fluxos de usuários de identidade B2C.|
|b2xUserFlows|Coleção [b2xIdentityUserFlow](b2xIdentityUserFlow.md)| Representa o ponto de entrada para fluxos de usuário de identidade de inscrição de autoatendimento e B2X.|
|identityProviders|Coleção [identityProviderBase](identityProviderBase.md)| Representa o ponto de entrada para a base do provedor de identidade.|
|userFlowAttributes|Coleção [identityUserFlowAttribute](identityUserFlowAttribute.md)| Representa o ponto de entrada para os atributos de fluxo de usuários de identidade.|
|continuousAccessEvaluationPolicy|[continuousAccessEvaluationPolicy](continuousAccessEvaluationPolicy.md)| Representa o ponto de entrada para a política de avaliação de acesso contínuo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityContainer"
}
```
