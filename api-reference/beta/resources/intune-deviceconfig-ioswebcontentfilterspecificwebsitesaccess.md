---
title: tipo de recurso de iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS. Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
ms.openlocfilehash: c5e23905ab9e5b692500544161fc052dd606da5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037435"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>tipo de recurso de iosWebContentFilterSpecificWebsitesAccess

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS. Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.

Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|specificWebsitesOnly|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|
|websiteList|coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|

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





