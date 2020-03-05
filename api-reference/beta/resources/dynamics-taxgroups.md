---
title: tipo de recurso taxGroups
description: Um objeto de grupo de impostos no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3c8f244b9c3601aaeb315b09bb51d21275a63f6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503254"
---
# <a name="taxgroups-resource-type"></a>tipo de recurso taxGroups

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso taxGroups no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter taxGroups](../api/dynamics-taxgroups-get.md)|taxGroups|Obtém um objeto de grupo de impostos.|
|[Postar taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|Cria um objeto de grupo de impostos.|
|[Patch taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|Atualiza um objeto de grupo de impostos.|
|[Excluir taxGroups](../api/dynamics-taxgroups-delete.md)|nenhuma|Exclui um objeto de grupo de impostos.|

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


