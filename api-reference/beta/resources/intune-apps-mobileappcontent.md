---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57266335608e97924edbddc056d931725a633e4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939116"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="8ead9-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="8ead9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ead9-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ead9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ead9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ead9-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8ead9-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ead9-108">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ead9-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="8ead9-109">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="8ead9-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="8ead9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ead9-110">Methods</span></span>
|<span data-ttu-id="8ead9-111">Método</span><span class="sxs-lookup"><span data-stu-id="8ead9-111">Method</span></span>|<span data-ttu-id="8ead9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ead9-112">Return Type</span></span>|<span data-ttu-id="8ead9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ead9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ead9-114">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="8ead9-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="8ead9-115">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="8ead9-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="8ead9-116">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8ead9-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="8ead9-117">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="8ead9-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8ead9-119">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8ead9-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8ead9-120">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="8ead9-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8ead9-122">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8ead9-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="8ead9-123">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="8ead9-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ead9-124">None</span></span>|<span data-ttu-id="8ead9-125">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8ead9-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="8ead9-126">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="8ead9-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="8ead9-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="8ead9-128">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="8ead9-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ead9-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ead9-129">Properties</span></span>
|<span data-ttu-id="8ead9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ead9-130">Property</span></span>|<span data-ttu-id="8ead9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ead9-131">Type</span></span>|<span data-ttu-id="8ead9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ead9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ead9-133">id</span><span class="sxs-lookup"><span data-stu-id="8ead9-133">id</span></span>|<span data-ttu-id="8ead9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ead9-134">String</span></span>|<span data-ttu-id="8ead9-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ead9-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ead9-136">Relações</span><span class="sxs-lookup"><span data-stu-id="8ead9-136">Relationships</span></span>
|<span data-ttu-id="8ead9-137">Relação</span><span class="sxs-lookup"><span data-stu-id="8ead9-137">Relationship</span></span>|<span data-ttu-id="8ead9-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ead9-138">Type</span></span>|<span data-ttu-id="8ead9-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ead9-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ead9-140">arquivos</span><span class="sxs-lookup"><span data-stu-id="8ead9-140">files</span></span>|<span data-ttu-id="8ead9-141">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="8ead9-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="8ead9-142">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ead9-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="8ead9-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="8ead9-143">containedApps</span></span>|<span data-ttu-id="8ead9-144">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8ead9-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="8ead9-145">A coleção de aplicativos contidos em um MobileLobApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="8ead9-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ead9-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ead9-146">JSON Representation</span></span>
<span data-ttu-id="8ead9-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ead9-147">Here is a JSON representation of the resource.</span></span>
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





