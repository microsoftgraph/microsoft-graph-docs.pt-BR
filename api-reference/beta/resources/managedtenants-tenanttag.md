---
title: Tipo de recurso tenantTag
description: Representa uma marca que pode ser atribuída ao locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: fa62dd86f14a85f6a7a8c4eaf9d722909f03981e
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862601"
---
# <a name="tenanttag-resource-type"></a>Tipo de recurso tenantTag

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma marca que pode ser atribuída ao locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tenantTags](../api/managedtenants-managedtenant-list-tenanttags.md)|[coleção microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Obter uma lista dos objetos [tenantTag](../resources/managedtenants-tenanttag.md) e suas propriedades.|
|[Criar tenantTag](../api/managedtenants-managedtenant-post-tenanttags.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Crie um novo [objeto tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Obter tenantTag](../api/managedtenants-tenanttag-get.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Leia as propriedades e as relações de um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Atualizar tenantTag](../api/managedtenants-tenanttag-update.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Atualize as propriedades de um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)|
|[Excluir tenantTag](../api/managedtenants-tenanttag-delete.md)|Nenhum|Exclui um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)|
|[assignTag](../api/managedtenants-tenanttag-assigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Atribui a marca de locatário aos locatários gerenciados especificados.|
|[unassignTag](../api/managedtenants-tenanttag-unassigntag.md)|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Não atribui a marca de locatário dos locatários gerenciados especificados.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdByUserId|String|O identificador da conta que criou a marca de locatário. Obrigatório. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora em que a marca de locatário foi criada. Obrigatório. Somente leitura.|
|deletedDateTime|DateTimeOffset|A data e a hora em que a marca de locatário foi excluída. Obrigatório. Somente leitura.|
|description|String|A descrição da marca de locatário. Opcional. Somente leitura.|
|displayName|String|O nome de exibição da marca de locatário. Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo da marca de locatário. Obrigatório. Somente leitura.|
|lastActionByUserId|String|O identificador da conta que durou na marca de locatário. Opcional. Somente leitura.|
|lastActionDateTime|DateTimeOffset|A data e a hora em que a última ação foi executada contra a marca de locatário. Opcional. Somente leitura.|
|locatários|[coleção microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)|A coleção de locatários gerenciados associados à marca de locatário. Opcional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantTag",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdByUserId": "String",
  "lastActionByUserId": "String",
  "tenants": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
    }
  ],
  "lastActionDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)"
}
```
