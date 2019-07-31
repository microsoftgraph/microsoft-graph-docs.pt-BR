---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b974f8a0ed243c454eef7fc1a51598b16c5fc57f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005153"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="7408e-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="7408e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7408e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7408e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7408e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7408e-107">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7408e-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="7408e-108">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="7408e-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="7408e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7408e-109">Methods</span></span>
|<span data-ttu-id="7408e-110">Método</span><span class="sxs-lookup"><span data-stu-id="7408e-110">Method</span></span>|<span data-ttu-id="7408e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7408e-111">Return Type</span></span>|<span data-ttu-id="7408e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7408e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7408e-113">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="7408e-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="7408e-114">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="7408e-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="7408e-115">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7408e-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="7408e-116">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="7408e-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="7408e-118">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7408e-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="7408e-119">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="7408e-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="7408e-121">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7408e-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="7408e-122">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="7408e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7408e-123">None</span></span>|<span data-ttu-id="7408e-124">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7408e-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="7408e-125">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="7408e-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7408e-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="7408e-127">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7408e-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7408e-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7408e-128">Properties</span></span>
|<span data-ttu-id="7408e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7408e-129">Property</span></span>|<span data-ttu-id="7408e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7408e-130">Type</span></span>|<span data-ttu-id="7408e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7408e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7408e-132">id</span><span class="sxs-lookup"><span data-stu-id="7408e-132">id</span></span>|<span data-ttu-id="7408e-133">String</span><span class="sxs-lookup"><span data-stu-id="7408e-133">String</span></span>|<span data-ttu-id="7408e-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7408e-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7408e-135">Relações</span><span class="sxs-lookup"><span data-stu-id="7408e-135">Relationships</span></span>
|<span data-ttu-id="7408e-136">Relação</span><span class="sxs-lookup"><span data-stu-id="7408e-136">Relationship</span></span>|<span data-ttu-id="7408e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="7408e-137">Type</span></span>|<span data-ttu-id="7408e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7408e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7408e-139">arquivos</span><span class="sxs-lookup"><span data-stu-id="7408e-139">files</span></span>|<span data-ttu-id="7408e-140">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="7408e-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="7408e-141">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7408e-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="7408e-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="7408e-142">containedApps</span></span>|<span data-ttu-id="7408e-143">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7408e-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="7408e-144">A coleção de aplicativos contidos em um MobileLobApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="7408e-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7408e-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7408e-145">JSON Representation</span></span>
<span data-ttu-id="7408e-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7408e-146">Here is a JSON representation of the resource.</span></span>
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





