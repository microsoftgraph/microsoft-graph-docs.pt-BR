---
title: tipo de recurso keyValue
description: Definição do valor da chave.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3133962d9f6bfb5f5363dd6d6cbd4b5ef2ea202
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406812"
---
# <a name="keyvalue-resource-type"></a>tipo de recurso keyValue

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Definição do valor da chave.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|key|String|Chave.|
|valor|Cadeia de caracteres|Valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




