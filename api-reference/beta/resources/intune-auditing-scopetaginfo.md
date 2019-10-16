---
title: tipo de recurso scopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8238881d8a14cb8aa1dfcc01031105be0069c21
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538501"
---
# <a name="scopetaginfo-resource-type"></a>tipo de recurso scopeTagInfo

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades do objeto de marca de escopo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|scopeTagName|Cadeia de caracteres|Nome de exibição da marca de escopo.|
|scopeTagId|Cadeia de caracteres|ID da marca de escopo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopeTagInfo",
  "scopeTagName": "String",
  "scopeTagId": "String"
}
```



