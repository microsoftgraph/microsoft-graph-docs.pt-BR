---
title: Tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas do SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59c76431ab5812bce62a417297339ee46c59691e80d2f84035cc801ed70f8af6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145373"
---
# <a name="configurationmanagerclientinformation-resource-type"></a>Tipo de recurso configurationManagerClientInformation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações do cliente do Configuration Manager sincronizadas do SCCM

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|clientIdentifier|Cadeia de caracteres|ID do cliente do Configuration Manager do SCCM|
|isBlocked|Boolean|Status bloqueado do Cliente do Gerenciador de Configurações do SCCM|

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
  "clientIdentifier": "String",
  "isBlocked": true
}
```




