---
title: tipo de recurso iosWebContentFilterSpecificWebsitesAccess
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS. Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd1e550b465f09676b3fe686f48dcfcec35e4bfe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702478"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="25b7b-104">tipo de recurso iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="25b7b-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="25b7b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b7b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25b7b-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25b7b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25b7b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25b7b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b7b-108">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS.</span><span class="sxs-lookup"><span data-stu-id="25b7b-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="25b7b-109">Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.</span><span class="sxs-lookup"><span data-stu-id="25b7b-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="25b7b-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="25b7b-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25b7b-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25b7b-111">Properties</span></span>
|<span data-ttu-id="25b7b-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25b7b-112">Property</span></span>|<span data-ttu-id="25b7b-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="25b7b-113">Type</span></span>|<span data-ttu-id="25b7b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="25b7b-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b7b-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="25b7b-115">specificWebsitesOnly</span></span>|<span data-ttu-id="25b7b-116">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="25b7b-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="25b7b-117">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="25b7b-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="25b7b-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="25b7b-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25b7b-119">websitelist</span><span class="sxs-lookup"><span data-stu-id="25b7b-119">websiteList</span></span>|<span data-ttu-id="25b7b-120">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="25b7b-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="25b7b-121">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="25b7b-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="25b7b-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="25b7b-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25b7b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="25b7b-123">Relationships</span></span>
<span data-ttu-id="25b7b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25b7b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25b7b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25b7b-125">JSON Representation</span></span>
<span data-ttu-id="25b7b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25b7b-126">Here is a JSON representation of the resource.</span></span>
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





