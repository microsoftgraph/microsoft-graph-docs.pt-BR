---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4b88a472912fab46011c7e030bb149bb2aed86a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527460"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="00b01-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-104">deviceCategory resource type</span></span>

<span data-ttu-id="00b01-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00b01-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00b01-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00b01-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00b01-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00b01-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00b01-108">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="00b01-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="00b01-109">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="00b01-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="00b01-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00b01-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="00b01-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00b01-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="00b01-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="00b01-112">Methods</span></span>
|<span data-ttu-id="00b01-113">Método</span><span class="sxs-lookup"><span data-stu-id="00b01-113">Method</span></span>|<span data-ttu-id="00b01-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00b01-114">Return Type</span></span>|<span data-ttu-id="00b01-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="00b01-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00b01-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="00b01-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="00b01-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="00b01-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="00b01-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="00b01-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="00b01-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="00b01-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="00b01-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="00b01-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="00b01-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="00b01-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="00b01-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="00b01-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="00b01-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="00b01-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="00b01-126">None</span></span>|<span data-ttu-id="00b01-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="00b01-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="00b01-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="00b01-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="00b01-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="00b01-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="00b01-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00b01-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00b01-131">Properties</span></span>
|<span data-ttu-id="00b01-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00b01-132">Property</span></span>|<span data-ttu-id="00b01-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="00b01-133">Type</span></span>|<span data-ttu-id="00b01-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="00b01-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b01-135">id</span><span class="sxs-lookup"><span data-stu-id="00b01-135">id</span></span>|<span data-ttu-id="00b01-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00b01-136">String</span></span>|<span data-ttu-id="00b01-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00b01-137">Unique identifier for the device category.</span></span> <span data-ttu-id="00b01-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00b01-138">Read-only.</span></span>|
|<span data-ttu-id="00b01-139">**Integração**</span><span class="sxs-lookup"><span data-stu-id="00b01-139">**Onboarding**</span></span>|
|<span data-ttu-id="00b01-140">displayName</span><span class="sxs-lookup"><span data-stu-id="00b01-140">displayName</span></span>|<span data-ttu-id="00b01-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00b01-141">String</span></span>|<span data-ttu-id="00b01-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00b01-142">Display name for the device category.</span></span>|
|<span data-ttu-id="00b01-143">description</span><span class="sxs-lookup"><span data-stu-id="00b01-143">description</span></span>|<span data-ttu-id="00b01-144">String</span><span class="sxs-lookup"><span data-stu-id="00b01-144">String</span></span>|<span data-ttu-id="00b01-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00b01-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00b01-146">Relações</span><span class="sxs-lookup"><span data-stu-id="00b01-146">Relationships</span></span>
<span data-ttu-id="00b01-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00b01-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00b01-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00b01-148">JSON Representation</span></span>
<span data-ttu-id="00b01-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00b01-149">Here is a JSON representation of the resource.</span></span>
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



