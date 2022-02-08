---
title: Tipo de recurso crossTenantAccessPolicyInboundTrust
description: Define as declarações de Acesso Condicional que você deseja aceitar de outras organizações por meio da configuração da política de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>Tipo de recurso crossTenantAccessPolicyInboundTrust

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as declarações de Acesso Condicional que você deseja aceitar de outras organizações do Azure AD por meio da configuração da política de acesso entre locatários. Eles podem ser configurados em sua configuração padrão, configuração específica do parceiro ou ambos.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| isCompliantDeviceAccepted | Boolean | Especifica se dispositivos compatíveis de organizações externas do Azure AD são confiáveis. |
| isHybridAzureADJoinedDeviceAccepted | Boolean | Especifica se os dispositivos do Azure AD híbridos ingressados em organizações externas do Azure AD são confiáveis. |
| isMfaAccepted | Boolean | Especifica se o MFA de organizações externas do Azure AD é confiável.|

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
