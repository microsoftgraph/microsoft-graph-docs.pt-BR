---
title: Tipo de recurso macOSAssociatedDomainsItem
description: Um mapeamento de identificadores de aplicativos para domínios associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2658a02a4881e793879a68bc6d1822d9a9b2a0a5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819140"
---
# <a name="macosassociateddomainsitem-resource-type"></a>Tipo de recurso macOSAssociatedDomainsItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um mapeamento de identificadores de aplicativos para domínios associados.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|applicationIdentifier|Cadeia de caracteres|O identificador de aplicativo do aplicativo ao que associar domínios.|
|domínios|Coleção de cadeias de caracteres|A lista de domínios a ser associado.|
|directDownloadsEnabled|Booliano|Determina se os dados devem ser baixados diretamente ou por meio de um CDN.|

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



