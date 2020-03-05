---
title: tipo de recurso unitsOfMeasure
description: Um objeto de unidade de medida no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9b0774f24109f40684039bd8ac98188903f28c3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503009"
---
# <a name="unitsofmeasure-resource-type"></a>tipo de recurso unitsOfMeasure

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma unidade de medida, que é um padrão de medida de uma quantidade, no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter unitsOfMeasure](../api/dynamics-unitsofmeasure-get.md)|unitsOfMeasure|Obtém um objeto de unidade de medida.|
|[Postar unitsOfMeasure](../api/dynamics-create-unitsofmeasure.md)|unitsOfMeasure|Cria um objeto de unidade de medida.|
|[Patch unitsOfMeasure](../api/dynamics-unitsofmeasure-update.md)|unitsOfMeasure|Atualiza um objeto de unidade de medida.|
|[Excluir unitsOfMeasure](../api/dynamics-unitsofmeasure-delete.md)|nenhuma|Exclui um objeto de unidade de medida.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|GUID|A ID exclusiva do unitsOfMeasure. Não editável.|
|código|cadeia de caracteres|Especifica o código da unidade de medida.|
|displayName|string|Especifica a unidade de nome de exibição da medida.|
|internationalStandardCode|string|Especifica a unidade de código de medida expressa de acordo com o padrão UNECE Rec20 em conexão com o envio eletrônico de documentos de vendas.|
|lastModifiedDateTime|datetime|O último DateTime em que a unidade de medida foi modificada. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso **unitsOfMeasure** .

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
