---
title: Tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5afd93641e68fa9b855c2a0003bc9192320eefac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137557"
---
# <a name="win32lobappreturncode-resource-type"></a>Tipo de recurso win32LobAppReturnCode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de código de retorno para um aplicativo Win32

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|returnCode|Int32|Código de retorno.|
|tipo|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|O tipo de código de retorno. Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




