---
title: tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe154ed3150ae434f8068bc04a56dd6e5b48744
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573057"
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
|enrollmentError|String|Erro de registro do conector de certificado|
|lastConnectorConnectionTime|DateTimeOffset|Última vez em que o conector de certificado está conectado|
|connectorVersion|String|Versão do conector de certificado|
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





