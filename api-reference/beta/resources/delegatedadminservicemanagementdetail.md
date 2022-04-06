---
title: Tipo de recurso delegatedAdminServiceManagementDetail
description: Contém os detalhes de gerenciamento de um serviço no locatário do cliente gerenciado pela administração delegada.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 837a7377031b7b2b913cf9346f8ca151da0267e1
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589531"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>Tipo de recurso delegatedAdminServiceManagementDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os detalhes de gerenciamento de um serviço no locatário do cliente gerenciado pela administração delegada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Obter uma lista dos **objetos delegatedAdminServiceManagementDetail** e suas propriedades.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador de um serviço gerenciado. Somente leitura.|
|serviceName|String|O nome de um serviço gerenciado. Somente leitura.|
|serviceManagementUrl|Cadeia de caracteres|A URL do portal de gerenciamento do serviço gerenciado. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminServiceManagementDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
  "id": "String (identifier)",
  "serviceName": "String",
  "serviceManagementUrl": "String"
}
```
