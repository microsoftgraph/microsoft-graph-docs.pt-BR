---
title: tipo de recurso crossTenantAccessPolicyConfigurationDefault
description: A configuração padrão definida para configurações de entrada e saída da colaboração do Azure AD B2B e conexão direta B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>tipo de recurso crossTenantAccessPolicyConfigurationDefault

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A configuração padrão definida para configurações de entrada e saída da colaboração do Azure AD B2B e conexão direta B2B.

Herda [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Obter a configuração padrão para a colaboração B2B e configurações de entrada e saída de conexão direta B2B.|
|[Atualizar crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|Nenhum|Atualize a configuração padrão para a colaboração B2B e configurações de entrada e saída de conexão direta B2B.|
|[Redefinir para o padrão do sistema](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|Nenhum|Redefina a configuração padrão de uma política de acesso entre locatários às configurações padrão do sistema.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários de outras organizações acessando seus recursos por meio da colaboração do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio da colaboração B2B do Azure AD. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários de outras organizações acessando seus recursos por meio da conexão direta do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio da conexão direta do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração padrão para confiar em outras declarações de Acesso Condicional de organizações externas do Azure AD. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| isServiceDefault | Boolean | Se `true`, a configuração padrão é definida como a configuração padrão do sistema. Se `false`, as configurações padrão foram personalizadas. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
  "baseType": "microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
  "inboundTrust": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
  },
  "b2bCollaborationOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bCollaborationInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "isServiceDefault": "Boolean"
}
```
