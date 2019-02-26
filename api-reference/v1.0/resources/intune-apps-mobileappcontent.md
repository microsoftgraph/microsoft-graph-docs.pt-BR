---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261296"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="b4171-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="b4171-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4171-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4171-106">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b4171-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="b4171-107">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="b4171-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="b4171-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4171-108">Methods</span></span>
|<span data-ttu-id="b4171-109">Método</span><span class="sxs-lookup"><span data-stu-id="b4171-109">Method</span></span>|<span data-ttu-id="b4171-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4171-110">Return Type</span></span>|<span data-ttu-id="b4171-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4171-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4171-112">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="b4171-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="b4171-113">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="b4171-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="b4171-114">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4171-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="b4171-115">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="b4171-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b4171-117">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4171-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="b4171-118">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="b4171-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b4171-120">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4171-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="b4171-121">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="b4171-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4171-122">None</span></span>|<span data-ttu-id="b4171-123">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4171-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="b4171-124">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="b4171-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="b4171-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="b4171-126">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="b4171-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4171-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4171-127">Properties</span></span>
|<span data-ttu-id="b4171-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4171-128">Property</span></span>|<span data-ttu-id="b4171-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4171-129">Type</span></span>|<span data-ttu-id="b4171-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4171-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4171-131">id</span><span class="sxs-lookup"><span data-stu-id="b4171-131">id</span></span>|<span data-ttu-id="b4171-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4171-132">String</span></span>|<span data-ttu-id="b4171-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b4171-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4171-134">Relações</span><span class="sxs-lookup"><span data-stu-id="b4171-134">Relationships</span></span>
|<span data-ttu-id="b4171-135">Relação</span><span class="sxs-lookup"><span data-stu-id="b4171-135">Relationship</span></span>|<span data-ttu-id="b4171-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4171-136">Type</span></span>|<span data-ttu-id="b4171-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4171-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4171-138">arquivos</span><span class="sxs-lookup"><span data-stu-id="b4171-138">files</span></span>|<span data-ttu-id="b4171-139">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="b4171-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="b4171-140">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b4171-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4171-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4171-141">JSON Representation</span></span>
<span data-ttu-id="b4171-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4171-142">Here is a JSON representation of the resource.</span></span>
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



