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
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="b0c4d-104">tipo de recurso iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="b0c4d-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="b0c4d-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0c4d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0c4d-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0c4d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c4d-108">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que instala os indicadores de URL no navegador integrado do iOS.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="b0c4d-109">Um cenário de exemplo está na sala de aula em que os professores gostariam que os alunos navegassem sites por meio de marcadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="b0c4d-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="b0c4d-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0c4d-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c4d-111">Properties</span></span>
|<span data-ttu-id="b0c4d-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c4d-112">Property</span></span>|<span data-ttu-id="b0c4d-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c4d-113">Type</span></span>|<span data-ttu-id="b0c4d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c4d-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c4d-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="b0c4d-115">specificWebsitesOnly</span></span>|<span data-ttu-id="b0c4d-116">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="b0c4d-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b0c4d-117">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b0c4d-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b0c4d-119">websitelist</span><span class="sxs-lookup"><span data-stu-id="b0c4d-119">websiteList</span></span>|<span data-ttu-id="b0c4d-120">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="b0c4d-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="b0c4d-121">Os indicadores de URL que serão instalados no navegador interno e o usuário só poderão acessar sites através de indicadores.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="b0c4d-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0c4d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b0c4d-123">Relationships</span></span>
<span data-ttu-id="b0c4d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0c4d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c4d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c4d-125">JSON Representation</span></span>
<span data-ttu-id="b0c4d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c4d-126">Here is a JSON representation of the resource.</span></span>
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



