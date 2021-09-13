---
title: Tipo de recurso macOSAssociatedDomainsItem
description: Um mapeamento de identificadores de aplicativos para domínios associados.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1229706d524cb16c9c66c1acf4c7fb86e65ede0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081322"
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
|domínios|Conjunto de cadeias de caracteres|A lista de domínios a ser associado.|
|directDownloadsEnabled|Boolean|Determina se os dados devem ser baixados diretamente ou por meio de um CDN.|

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



