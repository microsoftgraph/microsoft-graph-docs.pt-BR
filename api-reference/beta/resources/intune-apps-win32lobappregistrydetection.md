---
title: tipo de recurso win32LobAppRegistryDetection
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169542"
---
# <a name="win32lobappregistrydetection-resource-type"></a>tipo de recurso win32LobAppRegistryDetection

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades do registro para detectar um aplicativo Win32


Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|check32BitOn64System|Boolean|Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits|
|Caminho-chave|String|O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32|
|valueName|String|O nome do valor do registro|
|Detecção|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|O tipo de detecção de dados do registro. Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operador|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para a detecção de dados do registro. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detecçaovalue|String|O valor de detecção do registro|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




