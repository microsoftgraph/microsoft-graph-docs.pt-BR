---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83474d02f877da01e5f4dd1076492d691b5097c6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949966"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="2ff4f-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="2ff4f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ff4f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff4f-107">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="2ff4f-108">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="2ff4f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ff4f-109">Methods</span></span>
|<span data-ttu-id="2ff4f-110">Método</span><span class="sxs-lookup"><span data-stu-id="2ff4f-110">Method</span></span>|<span data-ttu-id="2ff4f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ff4f-111">Return Type</span></span>|<span data-ttu-id="2ff4f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ff4f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ff4f-113">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="2ff4f-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="2ff4f-114">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="2ff4f-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="2ff4f-115">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2ff4f-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="2ff4f-116">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="2ff4f-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2ff4f-118">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2ff4f-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2ff4f-119">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="2ff4f-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2ff4f-121">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2ff4f-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2ff4f-122">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="2ff4f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ff4f-123">None</span></span>|<span data-ttu-id="2ff4f-124">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2ff4f-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="2ff4f-125">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="2ff4f-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2ff4f-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2ff4f-127">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="2ff4f-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ff4f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ff4f-128">Properties</span></span>
|<span data-ttu-id="2ff4f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ff4f-129">Property</span></span>|<span data-ttu-id="2ff4f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ff4f-130">Type</span></span>|<span data-ttu-id="2ff4f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ff4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff4f-132">id</span><span class="sxs-lookup"><span data-stu-id="2ff4f-132">id</span></span>|<span data-ttu-id="2ff4f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ff4f-133">String</span></span>|<span data-ttu-id="2ff4f-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ff4f-135">Relações</span><span class="sxs-lookup"><span data-stu-id="2ff4f-135">Relationships</span></span>
|<span data-ttu-id="2ff4f-136">Relação</span><span class="sxs-lookup"><span data-stu-id="2ff4f-136">Relationship</span></span>|<span data-ttu-id="2ff4f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ff4f-137">Type</span></span>|<span data-ttu-id="2ff4f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ff4f-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff4f-139">arquivos</span><span class="sxs-lookup"><span data-stu-id="2ff4f-139">files</span></span>|<span data-ttu-id="2ff4f-140">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="2ff4f-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="2ff4f-141">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="2ff4f-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="2ff4f-142">containedApps</span></span>|<span data-ttu-id="2ff4f-143">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ff4f-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="2ff4f-144">A coleção de aplicativos contidos em um MobileLobApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ff4f-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ff4f-145">JSON Representation</span></span>
<span data-ttu-id="2ff4f-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ff4f-146">Here is a JSON representation of the resource.</span></span>
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




