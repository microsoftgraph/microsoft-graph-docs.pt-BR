---
title: tipo de recurso de iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS. Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424760"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="f34e7-104">tipo de recurso de iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="f34e7-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="f34e7-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f34e7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f34e7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f34e7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f34e7-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f34e7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34e7-108">Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS.</span><span class="sxs-lookup"><span data-stu-id="f34e7-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="f34e7-109">Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.</span><span class="sxs-lookup"><span data-stu-id="f34e7-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="f34e7-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="f34e7-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f34e7-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f34e7-111">Properties</span></span>
|<span data-ttu-id="f34e7-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f34e7-112">Property</span></span>|<span data-ttu-id="f34e7-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f34e7-113">Type</span></span>|<span data-ttu-id="f34e7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f34e7-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34e7-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="f34e7-115">specificWebsitesOnly</span></span>|<span data-ttu-id="f34e7-116">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="f34e7-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="f34e7-117">Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores.</span><span class="sxs-lookup"><span data-stu-id="f34e7-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="f34e7-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f34e7-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f34e7-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="f34e7-119">websiteList</span></span>|<span data-ttu-id="f34e7-120">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="f34e7-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="f34e7-121">Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores.</span><span class="sxs-lookup"><span data-stu-id="f34e7-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="f34e7-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f34e7-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f34e7-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f34e7-123">Relationships</span></span>
<span data-ttu-id="f34e7-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f34e7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f34e7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f34e7-125">JSON Representation</span></span>
<span data-ttu-id="f34e7-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f34e7-126">Here is a JSON representation of the resource.</span></span>
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




