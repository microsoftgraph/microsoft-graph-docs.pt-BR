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
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="750d4-104">tipo de recurso de iosWebContentFilterSpecificWebsitesAccess</span><span class="sxs-lookup"><span data-stu-id="750d4-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="750d4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="750d4-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="750d4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="750d4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="750d4-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="750d4-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="750d4-108">Representa um tipo de configuração de filtro de conteúdo da Web, que instala os indicadores de URL no navegador de internas iOS iOS.</span><span class="sxs-lookup"><span data-stu-id="750d4-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="750d4-109">Um exemplo de cenário é na sala de aula onde professores gostaria de alunos para navegar sites por meio de indicadores de navegador configurados em seus dispositivos iOS e sem acesso a outros sites.</span><span class="sxs-lookup"><span data-stu-id="750d4-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>

<span data-ttu-id="750d4-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="750d4-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="750d4-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="750d4-111">Properties</span></span>
|<span data-ttu-id="750d4-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="750d4-112">Property</span></span>|<span data-ttu-id="750d4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="750d4-113">Type</span></span>|<span data-ttu-id="750d4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="750d4-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750d4-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="750d4-115">specificWebsitesOnly</span></span>|<span data-ttu-id="750d4-116">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="750d4-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="750d4-117">Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores.</span><span class="sxs-lookup"><span data-stu-id="750d4-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="750d4-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="750d4-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="750d4-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="750d4-119">websiteList</span></span>|<span data-ttu-id="750d4-120">coleção [iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)</span><span class="sxs-lookup"><span data-stu-id="750d4-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="750d4-121">Indicadores de URL que serão instalados no navegador interno e o usuário só tem permissão para acessar sites da Web por meio de indicadores.</span><span class="sxs-lookup"><span data-stu-id="750d4-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="750d4-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="750d4-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="750d4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="750d4-123">Relationships</span></span>
<span data-ttu-id="750d4-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="750d4-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="750d4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="750d4-125">JSON Representation</span></span>
<span data-ttu-id="750d4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="750d4-126">Here is a JSON representation of the resource.</span></span>
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





