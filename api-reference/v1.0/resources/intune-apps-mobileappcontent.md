---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7857fff950e4cd4d8a46b73a58d52c86f72eb215
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028935"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="8dae7-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="8dae7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8dae7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dae7-106">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8dae7-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="8dae7-107">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="8dae7-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="8dae7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8dae7-108">Methods</span></span>
|<span data-ttu-id="8dae7-109">Método</span><span class="sxs-lookup"><span data-stu-id="8dae7-109">Method</span></span>|<span data-ttu-id="8dae7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8dae7-110">Return Type</span></span>|<span data-ttu-id="8dae7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dae7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8dae7-112">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="8dae7-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="8dae7-113">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="8dae7-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="8dae7-114">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8dae7-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="8dae7-115">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="8dae7-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8dae7-117">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8dae7-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8dae7-118">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="8dae7-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8dae7-120">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8dae7-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8dae7-121">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="8dae7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8dae7-122">None</span></span>|<span data-ttu-id="8dae7-123">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8dae7-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="8dae7-124">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="8dae7-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8dae7-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8dae7-126">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8dae7-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dae7-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dae7-127">Properties</span></span>
|<span data-ttu-id="8dae7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dae7-128">Property</span></span>|<span data-ttu-id="8dae7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dae7-129">Type</span></span>|<span data-ttu-id="8dae7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dae7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dae7-131">id</span><span class="sxs-lookup"><span data-stu-id="8dae7-131">id</span></span>|<span data-ttu-id="8dae7-132">String</span><span class="sxs-lookup"><span data-stu-id="8dae7-132">String</span></span>|<span data-ttu-id="8dae7-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8dae7-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dae7-134">Relações</span><span class="sxs-lookup"><span data-stu-id="8dae7-134">Relationships</span></span>
|<span data-ttu-id="8dae7-135">Relação</span><span class="sxs-lookup"><span data-stu-id="8dae7-135">Relationship</span></span>|<span data-ttu-id="8dae7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dae7-136">Type</span></span>|<span data-ttu-id="8dae7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dae7-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dae7-138">arquivos</span><span class="sxs-lookup"><span data-stu-id="8dae7-138">files</span></span>|<span data-ttu-id="8dae7-139">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="8dae7-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="8dae7-140">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8dae7-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8dae7-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dae7-141">JSON Representation</span></span>
<span data-ttu-id="8dae7-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dae7-142">Here is a JSON representation of the resource.</span></span>
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



