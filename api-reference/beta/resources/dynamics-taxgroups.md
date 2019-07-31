---
title: tipo de recurso taxGroups
description: Um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 378d8c1d773eacb3339eba35d5d60cc7ef5f2400
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006602"
---
# <a name="taxgroups-resource-type"></a>tipo de recurso taxGroups
Representa um tipo de recurso taxGroups no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxGroups](../api/dynamics-taxgroups-get.md)|taxGroups|Obtém um objeto de grupo de impostos.|
|[Postar taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|Cria um objeto de grupo de impostos.|
|[Patch taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|Atualiza um objeto de grupo de impostos.|
|[Excluir taxGroups](../api/dynamics-taxgroups-delete.md)|none|Exclui um objeto de grupo de impostos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da taxGroup. Somente Leitura.|
|código|cadeia de caracteres|Especifica o grupo de impostos.|
|displayName|string|Especifica o nome de exibição do grupo de impostos.|
|taxType|string|Especifica o tipo de imposto para o grupo.|
|lastModifiedDateTime|DateTime|O último DateTime que o grupo de impostos foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON da taxGroup.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


