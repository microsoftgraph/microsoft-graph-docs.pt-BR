---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e630e9e15e98744b349edb3c2986ff1b36a01a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684390"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="d2886-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-104">deviceCategory resource type</span></span>

<span data-ttu-id="d2886-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2886-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2886-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2886-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2886-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2886-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2886-108">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d2886-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="d2886-109">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="d2886-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span> <span data-ttu-id="d2886-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2886-110">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="d2886-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2886-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="d2886-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2886-112">Methods</span></span>
|<span data-ttu-id="d2886-113">Método</span><span class="sxs-lookup"><span data-stu-id="d2886-113">Method</span></span>|<span data-ttu-id="d2886-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2886-114">Return Type</span></span>|<span data-ttu-id="d2886-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2886-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2886-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="d2886-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="d2886-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="d2886-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="d2886-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2886-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="d2886-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="d2886-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="d2886-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2886-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="d2886-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="d2886-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="d2886-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2886-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="d2886-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="d2886-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d2886-126">None</span></span>|<span data-ttu-id="d2886-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2886-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="d2886-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="d2886-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2886-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="d2886-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d2886-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2886-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2886-131">Properties</span></span>
|<span data-ttu-id="d2886-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2886-132">Property</span></span>|<span data-ttu-id="d2886-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2886-133">Type</span></span>|<span data-ttu-id="d2886-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2886-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2886-135">id</span><span class="sxs-lookup"><span data-stu-id="d2886-135">id</span></span>|<span data-ttu-id="d2886-136">String</span><span class="sxs-lookup"><span data-stu-id="d2886-136">String</span></span>|<span data-ttu-id="d2886-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2886-137">Unique identifier for the device category.</span></span> <span data-ttu-id="d2886-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2886-138">Read-only.</span></span>|
|<span data-ttu-id="d2886-139">**Integração**</span><span class="sxs-lookup"><span data-stu-id="d2886-139">**Onboarding**</span></span>|
|<span data-ttu-id="d2886-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d2886-140">displayName</span></span>|<span data-ttu-id="d2886-141">String</span><span class="sxs-lookup"><span data-stu-id="d2886-141">String</span></span>|<span data-ttu-id="d2886-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2886-142">Display name for the device category.</span></span>|
|<span data-ttu-id="d2886-143">description</span><span class="sxs-lookup"><span data-stu-id="d2886-143">description</span></span>|<span data-ttu-id="d2886-144">String</span><span class="sxs-lookup"><span data-stu-id="d2886-144">String</span></span>|<span data-ttu-id="d2886-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d2886-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2886-146">Relações</span><span class="sxs-lookup"><span data-stu-id="d2886-146">Relationships</span></span>
<span data-ttu-id="d2886-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2886-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2886-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2886-148">JSON Representation</span></span>
<span data-ttu-id="d2886-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2886-149">Here is a JSON representation of the resource.</span></span>
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





