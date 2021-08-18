---
title: Tipo de recurso macOSSystemExtension
description: Representa uma extensão específica do sistema macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b717373ab3400a392943de83d86562876c900d88176fba1d044a7e0bb94e5044
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236357"
---
# <a name="macossystemextension-resource-type"></a>Tipo de recurso macOSSystemExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão específica do sistema macOS.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|Cadeia de caracteres|Obtém ou define o identificador de equipe que foi usado para assinar a extensão do sistema.|
|bundleId|String|Obtém ou define o identificador de pacote da extensão do sistema.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




