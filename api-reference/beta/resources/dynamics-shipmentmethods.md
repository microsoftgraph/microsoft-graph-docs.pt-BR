---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d45153a08572f32f29128fd4d3f51638d71c951b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027066"
---
# <a name="shipmentmethods-resource-type"></a>tipo de recurso shipmentMethods

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter shipmentMethods](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|Obtém um método de remessa.|
|[Postar shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|Cria um método de remessa.|
|[Patch shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|Atualiza um método de remessa.|
|[Excluir shipmentMethods](../api/dynamics-shipmentmethods-delete.md)|Nenhuma|Exclui um método de remessa.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do shipmentMethod. Não editável.|
|código|cadeia de caracteres|Especifica o código do método de remessa.|
|displayName|string|Especifica o nome de exibição do método de remessa.|
|lastModifiedDateTime|datetime|O último DateTime que o método de remessa foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do shipmentMethod.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```




