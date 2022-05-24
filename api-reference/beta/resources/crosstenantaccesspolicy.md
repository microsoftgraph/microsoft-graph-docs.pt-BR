---
title: Tipo de recurso crossTenantAccessPolicy
description: A política de acesso entre locatários representa a política base no diretório para configurações de acesso entre locatários.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: beea220ebf3a0b12e40e56997c236b82fcb5d2fe
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653536"
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
| allowedCloudEndpoints | Coleção de cadeias de caracteres | Usado para especificar com quais nuvens da Microsoft uma organização gostaria de colaborar. Por padrão, esse valor está vazio. Os valores com suporte para este campo são: `microsoftonline.com`, `microsoftonline.us`e `partner.microsoftonline.cn`. |
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
  "definition": "String",
  "allowedCloudEndpoints": ["String"]
}
```
