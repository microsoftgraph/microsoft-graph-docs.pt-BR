---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
ms.openlocfilehash: e57c4c0823636143962ac5fe1c50f4377e731f84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036759"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="a0808-104">Tipo de recurso mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="a0808-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0808-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0808-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0808-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0808-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0808-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0808-108">Contém propriedades de conteúdo para uma versão específica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0808-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="a0808-109">Cada mobileAppContent pode ter vários mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="a0808-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="a0808-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0808-110">Methods</span></span>
|<span data-ttu-id="a0808-111">Método</span><span class="sxs-lookup"><span data-stu-id="a0808-111">Method</span></span>|<span data-ttu-id="a0808-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0808-112">Return Type</span></span>|<span data-ttu-id="a0808-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0808-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0808-114">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="a0808-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="a0808-115">Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a0808-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="a0808-116">Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a0808-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="a0808-117">Obter mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="a0808-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a0808-119">Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a0808-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a0808-120">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="a0808-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a0808-122">Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a0808-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="a0808-123">Excluir mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="a0808-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0808-124">None</span></span>|<span data-ttu-id="a0808-125">Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a0808-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="a0808-126">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="a0808-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a0808-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="a0808-128">Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="a0808-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0808-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0808-129">Properties</span></span>
|<span data-ttu-id="a0808-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0808-130">Property</span></span>|<span data-ttu-id="a0808-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0808-131">Type</span></span>|<span data-ttu-id="a0808-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0808-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0808-133">id</span><span class="sxs-lookup"><span data-stu-id="a0808-133">id</span></span>|<span data-ttu-id="a0808-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0808-134">String</span></span>|<span data-ttu-id="a0808-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0808-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0808-136">Relações</span><span class="sxs-lookup"><span data-stu-id="a0808-136">Relationships</span></span>
|<span data-ttu-id="a0808-137">Relação</span><span class="sxs-lookup"><span data-stu-id="a0808-137">Relationship</span></span>|<span data-ttu-id="a0808-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0808-138">Type</span></span>|<span data-ttu-id="a0808-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0808-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0808-140">arquivos</span><span class="sxs-lookup"><span data-stu-id="a0808-140">files</span></span>|<span data-ttu-id="a0808-141">Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="a0808-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="a0808-142">A lista dos arquivos desta versão de conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a0808-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="a0808-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="a0808-143">containedApps</span></span>|<span data-ttu-id="a0808-144">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a0808-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="a0808-145">A coleção de aplicativos contidos em um MobileLobApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="a0808-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0808-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0808-146">JSON Representation</span></span>
<span data-ttu-id="a0808-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0808-147">Here is a JSON representation of the resource.</span></span>
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





