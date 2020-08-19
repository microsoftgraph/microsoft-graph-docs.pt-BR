---
title: tipo de recurso filesecuritystate
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: e030ce95ef2b8c5f1af5424bfdd0e727f2d3e2f6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806538"
---
# <a name="filesecuritystate-resource-type"></a>tipo de recurso filesecuritystate

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre o arquivo (não processo) relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo contendo hashes de arquivo (criptográfico e diferencia local).|
|nome|String|Nome do arquivo (sem o caminho).|
|caminho|String|Caminho completo do arquivo/ImageFile.|
|riskScore|String|Geração de um provedor/Pontuação de risco calculado do arquivo de alerta. O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
