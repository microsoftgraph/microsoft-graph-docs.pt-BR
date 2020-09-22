---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08b2cba09a8b9dadc1d86e1d430b93440de21681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094383"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="8f46f-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-104">mobileAppContent resource type</span></span>

<span data-ttu-id="8f46f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f46f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f46f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f46f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f46f-107">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f46f-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="8f46f-108">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="8f46f-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="8f46f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f46f-109">Methods</span></span>
|<span data-ttu-id="8f46f-110">Método</span><span class="sxs-lookup"><span data-stu-id="8f46f-110">Method</span></span>|<span data-ttu-id="8f46f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f46f-111">Return Type</span></span>|<span data-ttu-id="8f46f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f46f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f46f-113">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="8f46f-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="8f46f-114">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="8f46f-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="8f46f-115">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8f46f-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="8f46f-116">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="8f46f-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8f46f-118">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8f46f-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8f46f-119">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="8f46f-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8f46f-121">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8f46f-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8f46f-122">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="8f46f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f46f-123">None</span></span>|<span data-ttu-id="8f46f-124">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8f46f-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="8f46f-125">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="8f46f-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8f46f-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8f46f-127">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8f46f-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f46f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f46f-128">Properties</span></span>
|<span data-ttu-id="8f46f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f46f-129">Property</span></span>|<span data-ttu-id="8f46f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f46f-130">Type</span></span>|<span data-ttu-id="8f46f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f46f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f46f-132">id</span><span class="sxs-lookup"><span data-stu-id="8f46f-132">id</span></span>|<span data-ttu-id="8f46f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f46f-133">String</span></span>|<span data-ttu-id="8f46f-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f46f-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f46f-135">Relações</span><span class="sxs-lookup"><span data-stu-id="8f46f-135">Relationships</span></span>
|<span data-ttu-id="8f46f-136">Relação</span><span class="sxs-lookup"><span data-stu-id="8f46f-136">Relationship</span></span>|<span data-ttu-id="8f46f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f46f-137">Type</span></span>|<span data-ttu-id="8f46f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f46f-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f46f-139">arquivos</span><span class="sxs-lookup"><span data-stu-id="8f46f-139">files</span></span>|<span data-ttu-id="8f46f-140">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="8f46f-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="8f46f-141">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f46f-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f46f-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f46f-142">JSON Representation</span></span>
<span data-ttu-id="8f46f-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f46f-143">Here is a JSON representation of the resource.</span></span>
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









