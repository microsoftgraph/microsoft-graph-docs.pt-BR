---
title: tipo de recurso dataSource
description: Entidade DataSource-classe base abstrata
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597530"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="29e6c-103">tipo de recurso dataSource</span><span class="sxs-lookup"><span data-stu-id="29e6c-103">dataSource resource type</span></span>

<span data-ttu-id="29e6c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="29e6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29e6c-105">A entidade dataSource é uma BaseClass abstrata usada para identificar fontes de conteúdo para descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="29e6c-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="29e6c-106">Methods</span><span class="sxs-lookup"><span data-stu-id="29e6c-106">Methods</span></span>

<span data-ttu-id="29e6c-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29e6c-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="29e6c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29e6c-108">Properties</span></span>

|<span data-ttu-id="29e6c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29e6c-109">Property</span></span>|<span data-ttu-id="29e6c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="29e6c-110">Type</span></span>|<span data-ttu-id="29e6c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29e6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e6c-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="29e6c-112">createdBy</span></span>|[<span data-ttu-id="29e6c-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="29e6c-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="29e6c-114">O usuário que criou a **fonte** de os.</span><span class="sxs-lookup"><span data-stu-id="29e6c-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="29e6c-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29e6c-115">createdDateTime</span></span>|<span data-ttu-id="29e6c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29e6c-116">DateTimeOffset</span></span>|<span data-ttu-id="29e6c-117">A data e a hora em que a **fonte** de dados foi criada.</span><span class="sxs-lookup"><span data-stu-id="29e6c-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="29e6c-118">displayName</span><span class="sxs-lookup"><span data-stu-id="29e6c-118">displayName</span></span>|<span data-ttu-id="29e6c-119">String</span><span class="sxs-lookup"><span data-stu-id="29e6c-119">String</span></span>|<span data-ttu-id="29e6c-120">O nome de exibição da **fonte de fontes**.</span><span class="sxs-lookup"><span data-stu-id="29e6c-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="29e6c-121">Este será o nome do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="29e6c-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="29e6c-122">id</span><span class="sxs-lookup"><span data-stu-id="29e6c-122">id</span></span>|<span data-ttu-id="29e6c-123">String</span><span class="sxs-lookup"><span data-stu-id="29e6c-123">String</span></span>| <span data-ttu-id="29e6c-124">A ID da **DataSource**.</span><span class="sxs-lookup"><span data-stu-id="29e6c-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="29e6c-125">Esta não é a ID do site real.</span><span class="sxs-lookup"><span data-stu-id="29e6c-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29e6c-126">Relações</span><span class="sxs-lookup"><span data-stu-id="29e6c-126">Relationships</span></span>

<span data-ttu-id="29e6c-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29e6c-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29e6c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29e6c-128">JSON representation</span></span>

<span data-ttu-id="29e6c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29e6c-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
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
