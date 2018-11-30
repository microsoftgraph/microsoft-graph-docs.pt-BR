---
title: tipo de recurso de teamsTabConfiguration (Open tipo)
description: As configurações que determinam o conteúdo de uma guia.
ms.openlocfilehash: b9a638692302dc8d301c3b14e50096b08891d821
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034375"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="ca4e9-103">tipo de recurso de teamsTabConfiguration (Open tipo)</span><span class="sxs-lookup"><span data-stu-id="ca4e9-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="ca4e9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca4e9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca4e9-106">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="ca4e9-107">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="ca4e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca4e9-108">Properties</span></span>

|<span data-ttu-id="ca4e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca4e9-109">Property</span></span>|<span data-ttu-id="ca4e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca4e9-110">Type</span></span>|<span data-ttu-id="ca4e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca4e9-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="ca4e9-112">entityId</span><span class="sxs-lookup"><span data-stu-id="ca4e9-112">entityId</span></span>   |   <span data-ttu-id="ca4e9-113">string</span><span class="sxs-lookup"><span data-stu-id="ca4e9-113">string</span></span> |  <span data-ttu-id="ca4e9-114">Identificador da entidade hospedados pelo provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="ca4e9-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="ca4e9-115">contentUrl</span></span> |   <span data-ttu-id="ca4e9-116">string</span><span class="sxs-lookup"><span data-stu-id="ca4e9-116">string</span></span> |  <span data-ttu-id="ca4e9-117">URL usada para processar o conteúdo da guia em equipes.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="ca4e9-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-118">Required.</span></span>    |
|  <span data-ttu-id="ca4e9-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="ca4e9-119">removeUrl</span></span>  |   <span data-ttu-id="ca4e9-120">string</span><span class="sxs-lookup"><span data-stu-id="ca4e9-120">string</span></span> |  <span data-ttu-id="ca4e9-121">Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="ca4e9-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="ca4e9-122">websiteUrl</span></span> |   <span data-ttu-id="ca4e9-123">string</span><span class="sxs-lookup"><span data-stu-id="ca4e9-123">string</span></span> |  <span data-ttu-id="ca4e9-124">URL para a exibição de conteúdo da guia fora equipes.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="ca4e9-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca4e9-125">JSON representation</span></span>

<span data-ttu-id="ca4e9-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca4e9-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
