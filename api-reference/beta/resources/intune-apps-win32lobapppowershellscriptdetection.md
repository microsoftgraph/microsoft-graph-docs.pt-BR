---
title: Tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c611f83d591805a7f728989edcd222f5ea690146
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111380"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>Tipo de recurso win32LobAppPowerShellScriptDetection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de script do PowerShell para detectar um aplicativo Win32


Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enforceSignatureCheck|Boleano|Um valor que indica se a verificação de assinatura é imposta|
|runAs32Bit|Boleano|Um valor que indica se esse script deve ser executado como 32 bits|
|scriptContent|Cadeia de Caracteres|O conteúdo de script codificado base64 para detectar o aplicativo Win32 Line of Business (LoB)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```



