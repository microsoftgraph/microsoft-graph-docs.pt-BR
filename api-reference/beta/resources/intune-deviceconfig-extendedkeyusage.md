---
title: tipo de recurso extendedKeyUsage
description: Definição de uso de chave estendida personalizada
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36752e9a2f86e68bd4ada1a342dc174726a684c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946949"
---
# <a name="extendedkeyusage-resource-type"></a>tipo de recurso extendedKeyUsage

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de uso de chave estendida personalizada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|Nome estendido do uso de chave|
|objectidentifier|Cadeia de caracteres|Identificador de objeto de uso estendido de chave|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




