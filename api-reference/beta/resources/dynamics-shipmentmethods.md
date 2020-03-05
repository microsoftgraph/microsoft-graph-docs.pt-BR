---
title: tipo de recurso shipmentMethods
description: Um método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 94ebd10ef87946b5333ec5a06d5edccadc298158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503569"
---
# <a name="shipmentmethods-resource-type"></a>tipo de recurso shipmentMethods

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um método de entrega no Dynamics 365 Business central, como no-break, FEDEX e DHL.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter shipmentMethods](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|Obtém um método de remessa.|
|[Postar shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|Cria um método de remessa.|
|[Patch shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|Atualiza um método de remessa.|
|[Excluir shipmentMethods](../api/dynamics-shipmentmethods-delete.md)|nenhuma|Exclui um método de remessa.|

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


