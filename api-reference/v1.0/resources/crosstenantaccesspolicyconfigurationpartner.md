---
title: Tipo de recurso crossTenantAccessPolicyConfigurationPartner
description: A configuração específica do parceiro definida para as configurações de entrada e saída Azure AD colaboração B2B e conexão direta B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86c9cb0d5009d8406c99fd38520dddb18936c2c8
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604554"
---
# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>Tipo de recurso crossTenantAccessPolicyConfigurationPartner

Namespace: microsoft.graph

A configuração específica do parceiro que é definida para as configurações de entrada e saída Azure AD colaboração de conexão direta B2B e B2B.

Para qualquer propriedade específica do parceiro, `null`ou seja, essas configurações herdarão o comportamento definido em suas configurações de acesso entre [locatários padrão](../resources/crosstenantaccesspolicyconfigurationdefault.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Listar parceiros](../api/crosstenantaccesspolicy-list-partners.md) | [coleção crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Obtenha uma lista de todas as configurações específicas do parceiro. |
| [Criar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Crie uma nova configuração específica do parceiro. |
| [Obter crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Leia as definições de configuração específicas do parceiro. |
| [Atualizar crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | Atualize as propriedades de uma configuração específica do parceiro. |
| [Excluir crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | Nenhum | Exclua a configuração específica do parceiro. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações que acessam seus recursos por meio Azure AD colaboração B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para os usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD colaboração B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários de outras organizações que acessam seus recursos por meio do Azure B2B Direct Connect. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define a configuração específica do parceiro para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD conexão direta B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração específica do parceiro para confiar em outras declarações de Acesso Condicional de organizações Azure AD externas. |
| isServiceProvider | Boolean | Identifica se a configuração específica do parceiro é um Provedor de Serviços de Nuvem para sua organização. |
| tenantId | String | O identificador de locatário para o parceiro Azure AD organização. Somente leitura. Chave.|

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
