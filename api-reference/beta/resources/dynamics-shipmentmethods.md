---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365497"
---
# <a name="shipmentmethods-resource-type"></a>tipo de recurso shipmentMethods
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
|código|string|Especifica o código do método de remessa.|
|displayName|string|Especifica o nome de exibição do método de remessa.|
|lastModifiedDateTime|DateTime|O último DateTime que o método de remessa foi modificado. Somente Leitura.|  


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


