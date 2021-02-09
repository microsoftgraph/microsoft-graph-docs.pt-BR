---
title: Tipo de recurso dataSource
description: Entidade Datasource - classe base abstrata
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161919"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="e1b39-103">Tipo de recurso dataSource</span><span class="sxs-lookup"><span data-stu-id="e1b39-103">dataSource resource type</span></span>

<span data-ttu-id="e1b39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b39-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1b39-105">A entidade dataSource é uma baseclass abstrata usada para identificar fontes de conteúdo para Descobertas e Descobertas.</span><span class="sxs-lookup"><span data-stu-id="e1b39-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="e1b39-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1b39-106">Methods</span></span>

<span data-ttu-id="e1b39-107">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="e1b39-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="e1b39-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1b39-108">Properties</span></span>

|<span data-ttu-id="e1b39-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1b39-109">Property</span></span>|<span data-ttu-id="e1b39-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1b39-110">Type</span></span>|<span data-ttu-id="e1b39-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1b39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b39-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="e1b39-112">createdBy</span></span>|[<span data-ttu-id="e1b39-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="e1b39-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e1b39-114">O usuário que criou **o dataSource**.</span><span class="sxs-lookup"><span data-stu-id="e1b39-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="e1b39-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1b39-115">createdDateTime</span></span>|<span data-ttu-id="e1b39-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1b39-116">DateTimeOffset</span></span>|<span data-ttu-id="e1b39-117">A data e a hora em **que o dataSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="e1b39-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="e1b39-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e1b39-118">displayName</span></span>|<span data-ttu-id="e1b39-119">String</span><span class="sxs-lookup"><span data-stu-id="e1b39-119">String</span></span>|<span data-ttu-id="e1b39-120">O nome de exibição **do dataSource**.</span><span class="sxs-lookup"><span data-stu-id="e1b39-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="e1b39-121">Esse será o nome do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e1b39-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="e1b39-122">id</span><span class="sxs-lookup"><span data-stu-id="e1b39-122">id</span></span>|<span data-ttu-id="e1b39-123">String</span><span class="sxs-lookup"><span data-stu-id="e1b39-123">String</span></span>| <span data-ttu-id="e1b39-124">A ID do **dataSource**.</span><span class="sxs-lookup"><span data-stu-id="e1b39-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="e1b39-125">Essa não é a ID do site real.</span><span class="sxs-lookup"><span data-stu-id="e1b39-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1b39-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e1b39-126">Relationships</span></span>

<span data-ttu-id="e1b39-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1b39-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1b39-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1b39-128">JSON representation</span></span>

<span data-ttu-id="e1b39-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1b39-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
