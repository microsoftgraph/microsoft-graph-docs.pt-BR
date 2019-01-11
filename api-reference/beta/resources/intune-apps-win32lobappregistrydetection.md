---
title: tipo de recurso de win32LobAppRegistryDetection
description: Contém propriedades do registro para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: faccc030a9f15b511af4123c94687c904e60ff10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867134"
---
# <a name="win32lobappregistrydetection-resource-type"></a>tipo de recurso de win32LobAppRegistryDetection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades do registro para detectar um aplicativo Win32

Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|check32BitOn64System|Booliano|Um valor indicando se nesse caminho do registro é para verificação de aplicativo de 32 bits no sistema de 64 bits|
|caminho-chave|Cadeia de caracteres|O caminho da chave do registro para detectar app Win32 linha de negócios (LoB)|
|valueName|Cadeia de caracteres|O nome do valor do registro|
|tipo de detecção|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|O tipo de detecção de dados de registro. Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operador|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para detecção de dados de registro. Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Cadeia de caracteres|O valor de detecção do registro|

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





