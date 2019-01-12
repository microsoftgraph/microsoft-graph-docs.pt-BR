---
title: tipo de recurso de certificateConnectorSetting
description: Configurações do conector de certificado.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74a63d308d53d09b71b19b2ff10a9d94c3fa818d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980990"
---
# <a name="certificateconnectorsetting-resource-type"></a>tipo de recurso de certificateConnectorSetting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configurações do conector de certificado.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|status|Int32|Status do conector de certificado|
|certExpiryTime|DateTimeOffset|Certificado expirará tempo|
|enrollmentError|Cadeia de caracteres|Erro de inscrição do conector de certificado|
|lastConnectorConnectionTime|DateTimeOffset|Hora da última certificado conector conectado|
|connectorVersion|Cadeia de caracteres|Versão do conector de certificado|
|lastUploadVersion|Int64|Versão do conector do último certificado carregado|

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





