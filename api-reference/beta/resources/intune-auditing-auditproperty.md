---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27eda22c48f60da1cd224add29559b13505f7d8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004873"
---
# <a name="auditproperty-resource-type"></a>Tipo de recurso auditProperty

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades para a Propriedade de auditoria.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição.|
|oldValue|String|Valor antigo.|
|newValue|Cadeia de caracteres|Novo valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```





