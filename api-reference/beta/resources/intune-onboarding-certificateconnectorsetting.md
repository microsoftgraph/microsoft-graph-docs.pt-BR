---
title: Tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31b8ec7fcfe95e459e6454635b7b5e0a37c16cdec45eba5515a24165ad5ad80d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206246"
---
# <a name="certificateconnectorsetting-resource-type"></a>Tipo de recurso certificateConnectorSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações do conector de certificado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|status|Int32|Status do conector de certificado|
|certExpiryTime|DateTimeOffset|Tempo de expiração do certificado|
|enrollmentError|Cadeia de caracteres|Erro de registro do conector de certificado|
|lastConnectorConnectionTime|DateTimeOffset|Conector de certificado da última vez conectado|
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




