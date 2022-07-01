---
title: Tipo de recurso crossTenantAccessPolicy
description: A política de acesso entre locatários representa a política base no diretório para configurações de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2fb0f51f661938a3ee25edb4519fd5e8bc16987b
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604557"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>Tipo de recurso crossTenantAccessPolicy

Namespace: microsoft.graph

Representa a política base no diretório para configurações de acesso entre locatários.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Leia as propriedades e as relações de um [objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|
|[Atualizar crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Atualize as propriedades de [um objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| displayName | String | O nome de exibição da política de acesso entre locatários. Herdado do [policyBase](../resources/policybase.md).|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|Padrão.|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Define a configuração padrão de como sua organização interage com organizações externas do Azure Active Directory.|
|Parceiros|[coleção crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)|Define configurações específicas do parceiro para organizações externas do Azure Active Directory.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicy",
  "baseType": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicy",
  "displayName": "String"
}
```
