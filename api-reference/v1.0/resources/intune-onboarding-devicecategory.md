---
title: Tipo de recurso deviceCategory
description: Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas. Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5def5ee6c6a97e91c9255a9808db7fc6b2fa07fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751772"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="bf5ea-106">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-106">deviceCategory resource type</span></span>

<span data-ttu-id="bf5ea-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf5ea-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf5ea-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf5ea-109">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-109">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="bf5ea-110">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-110">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="bf5ea-111">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-111">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="bf5ea-112">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-112">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="bf5ea-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="bf5ea-113">Methods</span></span>
|<span data-ttu-id="bf5ea-114">Método</span><span class="sxs-lookup"><span data-stu-id="bf5ea-114">Method</span></span>|<span data-ttu-id="bf5ea-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bf5ea-115">Return Type</span></span>|<span data-ttu-id="bf5ea-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf5ea-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf5ea-117">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="bf5ea-117">List deviceCategories</span></span>](../api/intune-onboarding-devicecategory-list.md)|<span data-ttu-id="bf5ea-118">Coleção [deviceCategory](../resources/intune-onboarding-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="bf5ea-118">[deviceCategory](../resources/intune-onboarding-devicecategory.md) collection</span></span>|<span data-ttu-id="bf5ea-119">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bf5ea-119">List properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="bf5ea-120">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-120">Get deviceCategory</span></span>](../api/intune-onboarding-devicecategory-get.md)|[<span data-ttu-id="bf5ea-121">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-121">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="bf5ea-122">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bf5ea-122">Read properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="bf5ea-123">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-123">Create deviceCategory</span></span>](../api/intune-onboarding-devicecategory-create.md)|[<span data-ttu-id="bf5ea-124">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-124">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="bf5ea-125">Cria um novo objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bf5ea-125">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="bf5ea-126">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-126">Delete deviceCategory</span></span>](../api/intune-onboarding-devicecategory-delete.md)|<span data-ttu-id="bf5ea-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bf5ea-127">None</span></span>|<span data-ttu-id="bf5ea-128">Exclui um [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bf5ea-128">Deletes a [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span></span>|
|[<span data-ttu-id="bf5ea-129">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-129">Update deviceCategory</span></span>](../api/intune-onboarding-devicecategory-update.md)|[<span data-ttu-id="bf5ea-130">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bf5ea-130">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="bf5ea-131">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bf5ea-131">Update the properties of a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf5ea-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf5ea-132">Properties</span></span>
|<span data-ttu-id="bf5ea-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf5ea-133">Property</span></span>|<span data-ttu-id="bf5ea-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf5ea-134">Type</span></span>|<span data-ttu-id="bf5ea-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf5ea-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf5ea-136">id</span><span class="sxs-lookup"><span data-stu-id="bf5ea-136">id</span></span>|<span data-ttu-id="bf5ea-137">String</span><span class="sxs-lookup"><span data-stu-id="bf5ea-137">String</span></span>|<span data-ttu-id="bf5ea-138">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-138">Unique identifier for the device category.</span></span> <span data-ttu-id="bf5ea-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-139">Read-only.</span></span>|
|<span data-ttu-id="bf5ea-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bf5ea-140">displayName</span></span>|<span data-ttu-id="bf5ea-141">String</span><span class="sxs-lookup"><span data-stu-id="bf5ea-141">String</span></span>|<span data-ttu-id="bf5ea-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-142">Display name for the device category.</span></span>|
|<span data-ttu-id="bf5ea-143">description</span><span class="sxs-lookup"><span data-stu-id="bf5ea-143">description</span></span>|<span data-ttu-id="bf5ea-144">String</span><span class="sxs-lookup"><span data-stu-id="bf5ea-144">String</span></span>|<span data-ttu-id="bf5ea-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf5ea-146">Relações</span><span class="sxs-lookup"><span data-stu-id="bf5ea-146">Relationships</span></span>
<span data-ttu-id="bf5ea-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf5ea-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf5ea-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf5ea-148">JSON Representation</span></span>
<span data-ttu-id="bf5ea-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf5ea-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```




