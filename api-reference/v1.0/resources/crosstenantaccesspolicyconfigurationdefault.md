---
title: Tipo de recurso crossTenantAccessPolicyConfigurationDefault
description: A configuração padrão definida para as configurações de entrada e saída Azure AD colaboração B2B e conexão direta B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 08d32f51db26721205806b4b730ae6f77c0b4b98
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604555"
---
# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>Tipo de recurso crossTenantAccessPolicyConfigurationDefault

Namespace: microsoft.graph

A configuração padrão definida para as configurações de entrada e saída Azure AD colaboração B2B e conexão direta B2B.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Obtenha a configuração padrão para as configurações de entrada e saída de colaboração B2B e conexão direta B2B.|
|[Atualizar crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|Nenhum|Atualize a configuração padrão para as configurações de entrada e saída de colaboração B2B e conexão direta B2B.|
|[Redefinir para o padrão do sistema](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|Nenhum|Redefina a configuração padrão de uma política de acesso entre locatários para as configurações padrão do sistema.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários de outras organizações que acessam seus recursos por meio Azure AD colaboração B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD colaboração B2B. |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Define sua configuração padrão para usuários de outras organizações que acessam seus recursos por meio Azure AD conexão direta B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Define sua configuração padrão para usuários em sua organização que vão de saída para acessar recursos em outra organização por meio Azure AD conexão direta B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Determina a configuração padrão para confiar em outras declarações de Acesso Condicional de organizações Azure AD externas. |
| isServiceDefault | Boolean | If `true`, a configuração padrão é definida como a configuração padrão do sistema. If `false`, as configurações padrão foram personalizadas. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
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
