---
title: tipo de recurso iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32cf57ba7ab96a68914ceeaf0693162ef9ab8e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001051"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="964cc-104">tipo de recurso iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="964cc-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="964cc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="964cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="964cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="964cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="964cc-107">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS.</span><span class="sxs-lookup"><span data-stu-id="964cc-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="964cc-108">Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.</span><span class="sxs-lookup"><span data-stu-id="964cc-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="964cc-109">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="964cc-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="964cc-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="964cc-110">Properties</span></span>
|<span data-ttu-id="964cc-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="964cc-111">Property</span></span>|<span data-ttu-id="964cc-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="964cc-112">Type</span></span>|<span data-ttu-id="964cc-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="964cc-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="964cc-114">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="964cc-114">specificWebsitesOnly</span></span>|<span data-ttu-id="964cc-115">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="964cc-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="964cc-116">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="964cc-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="964cc-117">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="964cc-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="964cc-118">websitelist</span><span class="sxs-lookup"><span data-stu-id="964cc-118">websiteList</span></span>|<span data-ttu-id="964cc-119">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="964cc-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="964cc-120">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="964cc-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="964cc-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="964cc-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="964cc-122">Relações</span><span class="sxs-lookup"><span data-stu-id="964cc-122">Relationships</span></span>
<span data-ttu-id="964cc-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="964cc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="964cc-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="964cc-124">JSON Representation</span></span>
<span data-ttu-id="964cc-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="964cc-125">Here is a JSON representation of the resource.</span></span>
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





