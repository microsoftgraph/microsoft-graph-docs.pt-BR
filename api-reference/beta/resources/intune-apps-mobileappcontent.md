---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e88cab2a1d06ff31a64dbdf71de46e78068070d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076369"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="c1c0a-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-104">mobileAppContent resource type</span></span>

<span data-ttu-id="c1c0a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1c0a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1c0a-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1c0a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c0a-108">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="c1c0a-109">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="c1c0a-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1c0a-110">Methods</span></span>
|<span data-ttu-id="c1c0a-111">Método</span><span class="sxs-lookup"><span data-stu-id="c1c0a-111">Method</span></span>|<span data-ttu-id="c1c0a-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1c0a-112">Return Type</span></span>|<span data-ttu-id="c1c0a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c0a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1c0a-114">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="c1c0a-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="c1c0a-115">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="c1c0a-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="c1c0a-116">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0a-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="c1c0a-117">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="c1c0a-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c1c0a-119">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0a-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c1c0a-120">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="c1c0a-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c1c0a-122">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0a-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="c1c0a-123">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="c1c0a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1c0a-124">None</span></span>|<span data-ttu-id="c1c0a-125">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0a-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="c1c0a-126">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="c1c0a-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c1c0a-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="c1c0a-128">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c1c0a-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1c0a-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1c0a-129">Properties</span></span>
|<span data-ttu-id="c1c0a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1c0a-130">Property</span></span>|<span data-ttu-id="c1c0a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1c0a-131">Type</span></span>|<span data-ttu-id="c1c0a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c0a-133">id</span><span class="sxs-lookup"><span data-stu-id="c1c0a-133">id</span></span>|<span data-ttu-id="c1c0a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1c0a-134">String</span></span>|<span data-ttu-id="c1c0a-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c0a-136">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="c1c0a-136">Relationships</span></span>
|<span data-ttu-id="c1c0a-137">Relação</span><span class="sxs-lookup"><span data-stu-id="c1c0a-137">Relationship</span></span>|<span data-ttu-id="c1c0a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1c0a-138">Type</span></span>|<span data-ttu-id="c1c0a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c0a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c0a-140">arquivos</span><span class="sxs-lookup"><span data-stu-id="c1c0a-140">files</span></span>|<span data-ttu-id="c1c0a-141">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="c1c0a-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="c1c0a-142">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="c1c0a-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="c1c0a-143">containedApps</span></span>|<span data-ttu-id="c1c0a-144">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c1c0a-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="c1c0a-145">A coleção de aplicativos contidos em um MobileLobApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1c0a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1c0a-146">JSON Representation</span></span>
<span data-ttu-id="c1c0a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1c0a-147">Here is a JSON representation of the resource.</span></span>
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






