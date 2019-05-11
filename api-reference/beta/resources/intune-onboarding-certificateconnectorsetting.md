---
title: tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a980e6bf8dd97141fc3fc5a078beedbd0348a79
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940460"
---
# <a name="certificateconnectorsetting-resource-type"></a>tipo de recurso certificateConnectorSetting

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações do conector de certificado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|status|Int32|Status do conector de certificado|
|certExpiryTime|DateTimeOffset|Tempo de validade do certificado|
|enrollmentError|Cadeia de caracteres|Erro de registro do conector de certificado|
|lastConnectorConnectionTime|DateTimeOffset|Última vez em que o conector de certificado está conectado|
|connectorVersion|Cadeia de caracteres|Versão do conector de certificado|
|lastUploadVersion|Int64|Versão do último conector de certificado carregado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```




