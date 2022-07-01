---
title: Tipo de recurso crossTenantAccessPolicyInboundTrust
description: Define as declarações de Acesso Condicional que você deseja aceitar de outras organizações por meio de sua configuração de política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fef57d6a1ae940677d7d5412838223618d9aae66
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604553"
---
# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>Tipo de recurso crossTenantAccessPolicyInboundTrust

Namespace: microsoft.graph

Define as declarações de Acesso Condicional que você deseja aceitar de outras organizações Azure AD por meio de sua configuração de política de acesso entre locatários. Eles podem ser configurados em sua configuração padrão, configuração específica do parceiro ou ambos.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| isCompliantDeviceAccepted | Boolean | Especifica se os dispositivos compatíveis de organizações Azure AD externas são confiáveis. |
| isHybridAzureADJoinedDeviceAccepted | Boolean | Especifica se os dispositivos Azure AD ingressados em sistemas Azure AD externos são confiáveis. |
| isMfaAccepted | Boolean | Especifica se a MFA de organizações Azure AD externas é confiável.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyInboundTrust",
  "isMfaAccepted": "Boolean",
  "isCompliantDeviceAccepted": "Boolean",
  "isHybridAzureADJoinedDeviceAccepted": "Boolean"
}
```
