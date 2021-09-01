---
title: Tipo de recurso iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que instala indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula onde os professores gostaria que os alunos navegam em sites por meio de indicadores do navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbf2aeedc5ab9584cf65f00f665e1ba1340a9c15
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785749"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>Tipo de recurso iosWebContentFilterSpecificWebsitesAccess

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um tipo de configuração do Filtro de Conteúdo da Web do iOS, que instala indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula onde os professores gostaria que os alunos navegam em sites por meio de indicadores do navegador configurados em seus dispositivos iOS e sem acesso a outros sites.


Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|specificWebsitesOnly|[Coleção iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|
|websiteList|[Coleção iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)|Os indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites por meio de indicadores. Esta coleção pode conter um máximo de 500 elementos.|

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



