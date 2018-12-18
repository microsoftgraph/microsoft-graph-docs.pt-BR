---
title: tipo de recurso de teamsTabConfiguration (Open tipo)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
ms.openlocfilehash: 9abb4e9089da760825b29c4001b68881ab74d815
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301180"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="54f82-103">tipo de recurso de teamsTabConfiguration (Open tipo)</span><span class="sxs-lookup"><span data-stu-id="54f82-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="54f82-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="54f82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54f82-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54f82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54f82-106">As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="54f82-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="54f82-107">Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.</span><span class="sxs-lookup"><span data-stu-id="54f82-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="54f82-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54f82-108">Properties</span></span>

|<span data-ttu-id="54f82-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54f82-109">Property</span></span>|<span data-ttu-id="54f82-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="54f82-110">Type</span></span>|<span data-ttu-id="54f82-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="54f82-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="54f82-112">entityId</span><span class="sxs-lookup"><span data-stu-id="54f82-112">entityId</span></span>   |   <span data-ttu-id="54f82-113">string</span><span class="sxs-lookup"><span data-stu-id="54f82-113">string</span></span> |  <span data-ttu-id="54f82-114">Identificador da entidade hospedados pelo provedor de guia.</span><span class="sxs-lookup"><span data-stu-id="54f82-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="54f82-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="54f82-115">contentUrl</span></span> |   <span data-ttu-id="54f82-116">string</span><span class="sxs-lookup"><span data-stu-id="54f82-116">string</span></span> |  <span data-ttu-id="54f82-117">URL usada para processar o conteúdo da guia em equipes.</span><span class="sxs-lookup"><span data-stu-id="54f82-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="54f82-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54f82-118">Required.</span></span>    |
|  <span data-ttu-id="54f82-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="54f82-119">removeUrl</span></span>  |   <span data-ttu-id="54f82-120">string</span><span class="sxs-lookup"><span data-stu-id="54f82-120">string</span></span> |  <span data-ttu-id="54f82-121">Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.</span><span class="sxs-lookup"><span data-stu-id="54f82-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="54f82-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="54f82-122">websiteUrl</span></span> |   <span data-ttu-id="54f82-123">string</span><span class="sxs-lookup"><span data-stu-id="54f82-123">string</span></span> |  <span data-ttu-id="54f82-124">URL para a exibição de conteúdo da guia fora equipes.</span><span class="sxs-lookup"><span data-stu-id="54f82-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="54f82-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54f82-125">JSON representation</span></span>

<span data-ttu-id="54f82-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54f82-126">The following is a JSON representation of the resource.</span></span>
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
