---
title: tipo de recurso macOSAssociatedDomainsItem
description: Um mapeamento de identificadores de aplicativo para domínios associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fa40fda83eb6dd89fa0d8fd709a8bf744a8cc19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736251"
---
# <a name="macosassociateddomainsitem-resource-type"></a>tipo de recurso macOSAssociatedDomainsItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um mapeamento de identificadores de aplicativo para domínios associados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationIdentifier|String|O identificador de aplicativo do aplicativo para o qual associar domínios.|
|domínio|Coleção de cadeias de caracteres|A lista de domínios a serem associados.|
|directDownloadsEnabled|Booliano|Determina se os dados devem ser baixados diretamente ou por meio de uma CDN.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```





