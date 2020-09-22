---
title: tipo de recurso taxGroups
description: Um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 373e4785d19a7983f890ee3c3574533323829954
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027038"
---
# <a name="taxgroups-resource-type"></a>tipo de recurso taxGroups

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso taxGroups no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxGroups](../api/dynamics-taxgroups-get.md)|taxGroups|Obtém um objeto de grupo de impostos.|
|[Postar taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|Cria um objeto de grupo de impostos.|
|[Patch taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|Atualiza um objeto de grupo de impostos.|
|[Excluir taxGroups](../api/dynamics-taxgroups-delete.md)|Nenhuma|Exclui um objeto de grupo de impostos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A identificação exclusiva da taxGroup. Somente Leitura.|
|código|cadeia de caracteres|Especifica o grupo de impostos.|
|displayName|string|Especifica o nome de exibição do grupo de impostos.|
|taxType|string|Especifica o tipo de imposto para o grupo.|
|lastModifiedDateTime|datetime|O último DateTime que o grupo de impostos foi modificado. Somente leitura.|  


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




