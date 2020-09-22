---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97b56db5eb906d16b344e9e8c0a2bbb920cf5e46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060837"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a>tipo de recurso bulkManagedDeviceActionResult

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|successfulDeviceIds|Coleção de cadeias de caracteres|Dispositivos bem-sucedidos|
|failedDeviceIds|Coleção de cadeias de caracteres|Dispositivos com falha|
|notFoundDeviceIds|Coleção de cadeias de caracteres|Dispositivos não encontrados|
|notSupportedDeviceIds|Coleção de cadeias de caracteres|Dispositivos não suportados|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```






