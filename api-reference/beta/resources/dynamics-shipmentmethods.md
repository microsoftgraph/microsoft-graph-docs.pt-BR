---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006609"
---
# <a name="shipmentmethods-resource-type"></a>tipo de recurso shipmentMethods
Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter shipmentMethods](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|Obtém um método de remessa.|
|[Postar shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|Cria um método de remessa.|
|[Patch shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|Atualiza um método de remessa.|
|[Excluir shipmentMethods](../api/dynamics-shipmentmethods-delete.md)|none|Exclui um método de remessa.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do shipmentMethod. Não editável.|
|código|cadeia de caracteres|Especifica o código do método de remessa.|
|displayName|string|Especifica o nome de exibição do método de remessa.|
|lastModifiedDateTime|DateTime|O último DateTime que o método de remessa foi modificado. Somente leitura.|  


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


