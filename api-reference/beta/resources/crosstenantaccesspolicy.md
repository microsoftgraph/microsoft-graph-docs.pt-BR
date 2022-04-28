---
title: Tipo de recurso crossTenantAccessPolicy
description: A política de acesso entre locatários representa a política base no diretório para configurações de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ed825ae07c1a707be2847b9bdc40f7fe71add334
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103008"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>Tipo de recurso crossTenantAccessPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a política base no diretório para configurações de acesso entre locatários.

Herda de [tenantRelationshipAccessPolicyBase](../resources/tenantrelationshipaccesspolicybase.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Leia as propriedades e as relações de um [objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|
|[Atualizar crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Atualize as propriedades de [um objeto crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| displayName | Cadeia de caracteres | O nome de exibição da política de acesso entre locatários. Herdado do [policyBase](../resources/policybase.md).|
| definição (preterido) | Cadeia de caracteres | A definição JSON bruta da política de acesso entre locatários. **Preterido. Não use.**|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|Padrão.|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Define a configuração padrão de como sua organização interage com organizações Azure Active Directory externas.|
|Parceiros|[coleção crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)|Define configurações específicas do parceiro para organizações de Azure Active Directory externas.|

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
  "displayName": "String",
  "definition": "String"
}
```
