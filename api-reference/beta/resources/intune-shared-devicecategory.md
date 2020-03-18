---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5132299abde233f68bb2b47033008d2d40719fe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771352"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="72513-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-104">deviceCategory resource type</span></span>

> <span data-ttu-id="72513-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72513-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72513-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72513-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72513-107">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72513-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="72513-108">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="72513-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="72513-109">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72513-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="72513-110">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72513-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="72513-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="72513-111">Methods</span></span>
|<span data-ttu-id="72513-112">Método</span><span class="sxs-lookup"><span data-stu-id="72513-112">Method</span></span>|<span data-ttu-id="72513-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="72513-113">Return Type</span></span>|<span data-ttu-id="72513-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="72513-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72513-115">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="72513-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="72513-116">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="72513-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="72513-117">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="72513-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="72513-118">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="72513-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72513-120">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="72513-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="72513-121">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="72513-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72513-123">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="72513-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="72513-124">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="72513-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="72513-125">None</span></span>|<span data-ttu-id="72513-126">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="72513-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="72513-127">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="72513-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="72513-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="72513-129">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="72513-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72513-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72513-130">Properties</span></span>
|<span data-ttu-id="72513-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72513-131">Property</span></span>|<span data-ttu-id="72513-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="72513-132">Type</span></span>|<span data-ttu-id="72513-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="72513-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72513-134">id</span><span class="sxs-lookup"><span data-stu-id="72513-134">id</span></span>|<span data-ttu-id="72513-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72513-135">String</span></span>|<span data-ttu-id="72513-136">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72513-136">Unique identifier for the device category.</span></span> <span data-ttu-id="72513-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72513-137">Read-only.</span></span>|
|<span data-ttu-id="72513-138">**Integração**</span><span class="sxs-lookup"><span data-stu-id="72513-138">**Onboarding**</span></span>|
|<span data-ttu-id="72513-139">displayName</span><span class="sxs-lookup"><span data-stu-id="72513-139">displayName</span></span>|<span data-ttu-id="72513-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72513-140">String</span></span>|<span data-ttu-id="72513-141">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72513-141">Display name for the device category.</span></span>|
|<span data-ttu-id="72513-142">description</span><span class="sxs-lookup"><span data-stu-id="72513-142">description</span></span>|<span data-ttu-id="72513-143">String</span><span class="sxs-lookup"><span data-stu-id="72513-143">String</span></span>|<span data-ttu-id="72513-144">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72513-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72513-145">Relações</span><span class="sxs-lookup"><span data-stu-id="72513-145">Relationships</span></span>
<span data-ttu-id="72513-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72513-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72513-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72513-147">JSON Representation</span></span>
<span data-ttu-id="72513-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72513-148">Here is a JSON representation of the resource.</span></span>
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



