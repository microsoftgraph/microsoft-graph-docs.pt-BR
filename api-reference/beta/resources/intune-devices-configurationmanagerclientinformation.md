---
title: tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas a partir do SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b329d017aaf9f7d26d76f74198b2c5508e97ae2c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196977"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>tipo de recurso configurationManagerClientInformation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações do cliente do Configuration Manager sincronizadas a partir do SCCM

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|clientIdentifier|String|ID do cliente do Gerenciador de configurações do SCCM|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



