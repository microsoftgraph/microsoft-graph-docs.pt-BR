---
title: Tipo de recurso unifiedRbacResourceNamespace
description: Representa o namespace da área à qual a permissão de função pertence.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 85c290fc07c251864507ec34de0a4d6b6027b79e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338152"
---
# <a name="unifiedrbacresourcenamespace-resource-type"></a>Tipo de recurso unifiedRbacResourceNamespace

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o namespace da área ou serviço, como o Azure AD, o Intune e Exchange que define permissões de função.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRbacResourceNamespaces](../api/rbacapplicationmultiple-list-resourcenamespaces.md)|[Coleção unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Obter uma lista dos [objetos unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) e suas propriedades.|
|[Obter unifiedRbacResourceNamespace](../api/unifiedrbacresourcenamespace-get.md)|[unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md)|Leia as propriedades e as relações de um [objeto unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do namespace de recursos que define permissões, como `microsoft.aad.b2c`. Obrigatório.|
|nome|String|Nome do namespace do recurso. Normalmente, o mesmo nome da **propriedade id** , como `microsoft.aad.b2c`. Obrigatório. Suporta `$filter` (`eq`, `startsWith`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|resourceActions|[Coleção unifiedRbacResourceAction](unifiedrbacresourceaction.md)|Operações que uma entidade autorizada tem permissão para executar.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceNamespace",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceNamespace",
  "id": "String (identifier)",
  "name": "String"
}
```
