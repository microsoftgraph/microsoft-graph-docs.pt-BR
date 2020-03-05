---
title: tipo de recurso iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4129ce4f4332c78e5af6170b5ce48ab7aa19cee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529807"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>tipo de recurso iosWebContentFilterSpecificWebsitesAccess

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|specificWebsitesOnly|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores. Esta coleção pode conter um máximo de 500 elementos.|
|websitelist|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```



