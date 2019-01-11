---
title: Tipo de recurso de aplicativo
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
ms.openlocfilehash: a8e2124910301818e753b1f90a3168da3a072862
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804435"
---
# <a name="application-resource-type"></a>Tipo de recurso de aplicativo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o aplicativo Excel que gerencia a pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obtenha o aplicativo](../api/excelapplication-get.md) | [Application](application.md) |Leia as propriedades e os relacionamentos do objeto application.|
|[Calculate](../api/excelapplication-calculate.md)|Nenhum|Recalcula todas as pastas de trabalho abertas no Excel no momento.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|calculationMode|string|Retorna o modo de cálculo usado na pasta de trabalho. Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
