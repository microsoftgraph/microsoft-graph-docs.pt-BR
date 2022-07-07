---
title: Tipo de recurso win32LobAppPowerShellScriptRequirement
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0580328e628e8143b24ce6fecefb5e25b2218ac9
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668808"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>Tipo de recurso win32LobAppPowerShellScriptRequirement

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de script do PowerShell para detectar um aplicativo Win32


Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|O operador para detecção Herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Cadeia de caracteres|O valor de detecção Herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo para esta regra|
|enforceSignatureCheck|Boolean|Um valor que indica se a verificação de assinatura é imposta|
|runAs32Bit|Boolean|Um valor que indica se esse script deve ser executado como 32 bits|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|Indica o tipo de contexto de execução em que o script é executado. Os valores possíveis são: `system` e `user`.|
|scriptContent|Cadeia de caracteres|O conteúdo do script codificado em base64 para detectar o aplicativo Win32 Line of Business (LoB)|
|detectionType|[win32LobAppPowerShellScriptDetectionType](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|O tipo de detecção para a saída do script. Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```




