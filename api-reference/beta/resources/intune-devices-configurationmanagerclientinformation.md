---
title: Tipo de recurso configurationManagerClientInformation
description: Informações do cliente do Configuration Manager sincronizadas do SCCM
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3af9373c8359ed28465cb580057d06850dcb3504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026935"
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
|isBlocked|Booliano|Status bloqueado do Cliente do Gerenciador de Configurações do SCCM|

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



