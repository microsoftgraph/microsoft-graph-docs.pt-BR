---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ceeb6cd4e989f4e020c885dde119c39d9659539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418180"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="ea42c-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="ea42c-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea42c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ea42c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea42c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea42c-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ea42c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea42c-108">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea42c-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="ea42c-109">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ea42c-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="ea42c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea42c-110">Methods</span></span>
|<span data-ttu-id="ea42c-111">Método</span><span class="sxs-lookup"><span data-stu-id="ea42c-111">Method</span></span>|<span data-ttu-id="ea42c-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea42c-112">Return Type</span></span>|<span data-ttu-id="ea42c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea42c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea42c-114">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="ea42c-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="ea42c-115">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="ea42c-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="ea42c-116">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ea42c-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="ea42c-117">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="ea42c-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ea42c-119">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ea42c-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ea42c-120">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="ea42c-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ea42c-122">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ea42c-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="ea42c-123">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="ea42c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea42c-124">None</span></span>|<span data-ttu-id="ea42c-125">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ea42c-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="ea42c-126">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="ea42c-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="ea42c-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="ea42c-128">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="ea42c-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea42c-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea42c-129">Properties</span></span>
|<span data-ttu-id="ea42c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea42c-130">Property</span></span>|<span data-ttu-id="ea42c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea42c-131">Type</span></span>|<span data-ttu-id="ea42c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea42c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea42c-133">id</span><span class="sxs-lookup"><span data-stu-id="ea42c-133">id</span></span>|<span data-ttu-id="ea42c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea42c-134">String</span></span>|<span data-ttu-id="ea42c-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea42c-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea42c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="ea42c-136">Relationships</span></span>
|<span data-ttu-id="ea42c-137">Relação</span><span class="sxs-lookup"><span data-stu-id="ea42c-137">Relationship</span></span>|<span data-ttu-id="ea42c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea42c-138">Type</span></span>|<span data-ttu-id="ea42c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea42c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea42c-140">arquivos</span><span class="sxs-lookup"><span data-stu-id="ea42c-140">files</span></span>|<span data-ttu-id="ea42c-141">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="ea42c-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="ea42c-142">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea42c-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="ea42c-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="ea42c-143">containedApps</span></span>|<span data-ttu-id="ea42c-144">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea42c-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="ea42c-145">A coleção de aplicativos contidos em um MobileLobApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="ea42c-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea42c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea42c-146">JSON Representation</span></span>
<span data-ttu-id="ea42c-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea42c-147">Here is a JSON representation of the resource.</span></span>
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




