---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d0a97affa024a5a38e034b53a66b9c1c629cc96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354067"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="2d280-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="2d280-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d280-106">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d280-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="2d280-107">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="2d280-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="2d280-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d280-108">Methods</span></span>
|<span data-ttu-id="2d280-109">Método</span><span class="sxs-lookup"><span data-stu-id="2d280-109">Method</span></span>|<span data-ttu-id="2d280-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d280-110">Return Type</span></span>|<span data-ttu-id="2d280-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d280-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d280-112">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="2d280-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="2d280-113">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="2d280-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="2d280-114">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2d280-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="2d280-115">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="2d280-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2d280-117">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2d280-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2d280-118">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="2d280-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2d280-120">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2d280-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2d280-121">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="2d280-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d280-122">None</span></span>|<span data-ttu-id="2d280-123">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2d280-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="2d280-124">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="2d280-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2d280-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2d280-126">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2d280-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d280-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d280-127">Properties</span></span>
|<span data-ttu-id="2d280-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d280-128">Property</span></span>|<span data-ttu-id="2d280-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d280-129">Type</span></span>|<span data-ttu-id="2d280-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d280-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d280-131">id</span><span class="sxs-lookup"><span data-stu-id="2d280-131">id</span></span>|<span data-ttu-id="2d280-132">String</span><span class="sxs-lookup"><span data-stu-id="2d280-132">String</span></span>|<span data-ttu-id="2d280-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d280-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d280-134">Relações</span><span class="sxs-lookup"><span data-stu-id="2d280-134">Relationships</span></span>
|<span data-ttu-id="2d280-135">Relação</span><span class="sxs-lookup"><span data-stu-id="2d280-135">Relationship</span></span>|<span data-ttu-id="2d280-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d280-136">Type</span></span>|<span data-ttu-id="2d280-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d280-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d280-138">arquivos</span><span class="sxs-lookup"><span data-stu-id="2d280-138">files</span></span>|<span data-ttu-id="2d280-139">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="2d280-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="2d280-140">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d280-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d280-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d280-141">JSON Representation</span></span>
<span data-ttu-id="2d280-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d280-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




