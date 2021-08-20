---
title: Tipo de recurso macOSAssociatedDomainsItem
description: Um mapeamento de identificadores de aplicativos para domínios associados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff607e0eb88a53aa53500b278e7cbf90da49a34fa4033a3907f24818c3618ddc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183124"
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
|domínios|String collection|A lista de domínios a ser associado.|
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




