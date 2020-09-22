---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8091c873c18c1af0344cae9f6800e26e85181c19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081220"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>tipo de recurso managedDeviceCleanupSettings

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Defina a regra quando o administrador quiser que os dispositivos sejam limpos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|Cadeia de caracteres|Número de dias em que o dispositivo não entrou no Intune.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```






