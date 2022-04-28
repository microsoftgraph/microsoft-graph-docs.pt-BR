---
title: Tipo de recurso crossTenantAccessPolicyConfigurationPartner
description: A configuração específica do parceiro definida para as configurações de entrada e saída da colaboração B2B do Azure AD e da conexão direta B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 73849d18cce7639e82e5b56a37f46ce7705b707f
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103029"
---
# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>Tipo de recurso crossTenantAccessPolicyConfigurationPartner

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A configuração específica do parceiro definida para as configurações de entrada e saída da colaboração de conexão direta B2B e B2B do Azure AD.

Para qualquer propriedade específica do parceiro, `null`ou seja, essas configurações herdarão o comportamento definido em suas configurações de acesso entre [locatários padrão](../resources/crosstenantaccesspolicyconfigurationdefault.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar parceiros](../api/crosstenantaccesspolicy-list-partners.md) | [coleção crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Obtenha uma lista de todas as configurações específicas do parceiro. |
| [Criar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Crie uma nova configuração específica do parceiro. |
| [Obter crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Leia as definições de configuração específicas do parceiro. |
| [Atualizar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Atualize as propriedades de uma configuração específica do parceiro. |
| [Excluir crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | Nenhuma | Exclua a configuração específica do parceiro. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações que acessam seus recursos por meio da colaboração B2B do Azure AD. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio da colaboração B2B do Azure AD. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações que acessam seus recursos por meio do Azure B2B Direct Connect. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para os usuários em sua organização que vão de saída para acessar recursos em outra organização por meio do Azure AD B2B Direct Connect. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração específica do parceiro para confiar em outras declarações de Acesso Condicional de organizações externas do Azure AD. |
| isServiceProvider | Booliano | Identifica se a configuração específica do parceiro é um Provedor de Serviços de Nuvem para sua organização. |
| tenantId | String | O identificador de locatário da organização parceira do Azure AD. Somente leitura. Chave.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "tenantId",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "tenantId": "String (identifier)",
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
