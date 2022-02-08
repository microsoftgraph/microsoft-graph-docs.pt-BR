---
title: Tipo de recurso crossTenantAccessPolicyConfigurationPartner
description: A configuração específica do parceiro definida para configurações de entrada e saída da colaboração do Azure AD B2B e conexão direta B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>Tipo de recurso crossTenantAccessPolicyConfigurationPartner

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A configuração específica do parceiro definida para configurações de entrada e saída da colaboração de conexão direta do Azure AD B2B e B2B.

Para qualquer propriedade específica do parceiro que seja `null`, essas configurações herdarão o comportamento configurado em suas configurações de acesso entre [locatários padrão](../resources/crosstenantaccesspolicyconfigurationdefault.md).

Herda [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar parceiros](../api/crosstenantaccesspolicy-list-partners.md) | [Coleção crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Obter uma lista de todas as configurações específicas do parceiro. |
| [Criar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Crie uma nova configuração específica do parceiro. |
| [Obter crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Leia as configurações específicas do parceiro. |
| [Atualizar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Atualize as propriedades de uma configuração específica do parceiro. |
| [Excluir crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | Nenhum | Exclua a configuração específica do parceiro. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações acessando seus recursos por meio da colaboração do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio da colaboração do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações acessando seus recursos por meio de conexão direta do Azure B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio da conexão direta do Azure AD B2B. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração específica do parceiro para confiar em outras declarações de Acesso Condicional de organizações externas do Azure AD. Herdado [de crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| isServiceProvider | Boolean | Identifica se a configuração específica do parceiro é um Provedor de Serviços de Nuvem para sua organização. |
| tenantId | String | O identificador de locatário da organização do Azure AD do parceiro. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "baseType": "microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "tenantId": "String",
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
  "isServiceProvider": "Boolean"
}
```
