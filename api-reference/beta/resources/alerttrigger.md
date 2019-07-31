---
title: tipo de recurso alertTrigger
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 682ff7952b39cd71399441014c528eaba32ac4b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013386"
---
# <a name="alerttrigger-resource-type"></a>tipo de recurso alertTrigger

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre as propriedades que acionaram uma detecção (as propriedades existem na entidade de alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|name|String|Nome da propriedade servindo como um gatilho de detecção.|
|type|String|Tipo da propriedade no par chave: valor para interpretação. Por exemplo, String, Boolean, etc.|
|value|Cadeia de caracteres|O valor da propriedade servindo como um gatilho de detecção.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>Exemplo

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
