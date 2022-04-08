---
title: Tipo de recurso delegatedAdminServiceManagementDetail
description: Contém os detalhes de gerenciamento de um serviço no locatário do cliente gerenciado pela administração delegada.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 53eca1c8d8d60ea78e080caede5ed7096a6ff825
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704153"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>Tipo de recurso delegatedAdminServiceManagementDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os detalhes de gerenciamento de um serviço no locatário do cliente gerenciado pela administração delegada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar delegatedAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|Obtenha uma lista dos **objetos delegatedAdminServiceManagementDetail** e suas propriedades.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador de um serviço gerenciado. Somente leitura.|
|serviceName|Cadeia de caracteres|O nome de um serviço gerenciado. Somente leitura.|
|serviceManagementUrl|Cadeia de caracteres|A URL do portal de gerenciamento para o serviço gerenciado. Somente leitura.|

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
