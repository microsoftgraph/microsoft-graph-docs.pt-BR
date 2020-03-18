---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5cc1888288809812b0b2af533641fd61161cee08
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797843"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="eac36-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="eac36-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eac36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eac36-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eac36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac36-107">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eac36-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="eac36-108">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="eac36-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="eac36-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="eac36-109">Methods</span></span>
|<span data-ttu-id="eac36-110">Método</span><span class="sxs-lookup"><span data-stu-id="eac36-110">Method</span></span>|<span data-ttu-id="eac36-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eac36-111">Return Type</span></span>|<span data-ttu-id="eac36-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac36-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eac36-113">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="eac36-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="eac36-114">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="eac36-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="eac36-115">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="eac36-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="eac36-116">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="eac36-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="eac36-118">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="eac36-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="eac36-119">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="eac36-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="eac36-121">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="eac36-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="eac36-122">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="eac36-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eac36-123">None</span></span>|<span data-ttu-id="eac36-124">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="eac36-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="eac36-125">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="eac36-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="eac36-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="eac36-127">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="eac36-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eac36-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eac36-128">Properties</span></span>
|<span data-ttu-id="eac36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eac36-129">Property</span></span>|<span data-ttu-id="eac36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac36-130">Type</span></span>|<span data-ttu-id="eac36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac36-132">id</span><span class="sxs-lookup"><span data-stu-id="eac36-132">id</span></span>|<span data-ttu-id="eac36-133">String</span><span class="sxs-lookup"><span data-stu-id="eac36-133">String</span></span>|<span data-ttu-id="eac36-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eac36-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eac36-135">Relações</span><span class="sxs-lookup"><span data-stu-id="eac36-135">Relationships</span></span>
|<span data-ttu-id="eac36-136">Relação</span><span class="sxs-lookup"><span data-stu-id="eac36-136">Relationship</span></span>|<span data-ttu-id="eac36-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="eac36-137">Type</span></span>|<span data-ttu-id="eac36-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="eac36-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac36-139">arquivos</span><span class="sxs-lookup"><span data-stu-id="eac36-139">files</span></span>|<span data-ttu-id="eac36-140">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="eac36-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="eac36-141">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eac36-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="eac36-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="eac36-142">containedApps</span></span>|<span data-ttu-id="eac36-143">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="eac36-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="eac36-144">A coleção de aplicativos contidos em um MobileLobApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="eac36-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eac36-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eac36-145">JSON Representation</span></span>
<span data-ttu-id="eac36-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eac36-146">Here is a JSON representation of the resource.</span></span>
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



