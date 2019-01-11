---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cf1deeaf1a18d68675e68e7040099d31cdea552f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880294"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="29b84-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="29b84-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="29b84-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29b84-106">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29b84-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="29b84-107">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="29b84-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="29b84-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="29b84-108">Methods</span></span>
|<span data-ttu-id="29b84-109">Método</span><span class="sxs-lookup"><span data-stu-id="29b84-109">Method</span></span>|<span data-ttu-id="29b84-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29b84-110">Return Type</span></span>|<span data-ttu-id="29b84-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b84-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29b84-112">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="29b84-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="29b84-113">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="29b84-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="29b84-114">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="29b84-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="29b84-115">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="29b84-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="29b84-117">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="29b84-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="29b84-118">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="29b84-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="29b84-120">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="29b84-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="29b84-121">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="29b84-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29b84-122">None</span></span>|<span data-ttu-id="29b84-123">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="29b84-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="29b84-124">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="29b84-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="29b84-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="29b84-126">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="29b84-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29b84-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29b84-127">Properties</span></span>
|<span data-ttu-id="29b84-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29b84-128">Property</span></span>|<span data-ttu-id="29b84-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b84-129">Type</span></span>|<span data-ttu-id="29b84-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b84-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b84-131">id</span><span class="sxs-lookup"><span data-stu-id="29b84-131">id</span></span>|<span data-ttu-id="29b84-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29b84-132">String</span></span>|<span data-ttu-id="29b84-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29b84-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29b84-134">Relações</span><span class="sxs-lookup"><span data-stu-id="29b84-134">Relationships</span></span>
|<span data-ttu-id="29b84-135">Relação</span><span class="sxs-lookup"><span data-stu-id="29b84-135">Relationship</span></span>|<span data-ttu-id="29b84-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b84-136">Type</span></span>|<span data-ttu-id="29b84-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b84-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b84-138">arquivos</span><span class="sxs-lookup"><span data-stu-id="29b84-138">files</span></span>|<span data-ttu-id="29b84-139">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="29b84-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="29b84-140">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29b84-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29b84-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29b84-141">JSON Representation</span></span>
<span data-ttu-id="29b84-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29b84-142">Here is a JSON representation of the resource.</span></span>
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



