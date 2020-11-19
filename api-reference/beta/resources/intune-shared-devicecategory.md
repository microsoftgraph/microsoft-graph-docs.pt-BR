---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14ff0efe2532fd808e94c27c68777c4935212b01
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306895"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="b4b71-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-104">deviceCategory resource type</span></span>

<span data-ttu-id="b4b71-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4b71-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4b71-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4b71-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4b71-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4b71-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b71-108">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b4b71-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="b4b71-109">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="b4b71-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span> <span data-ttu-id="b4b71-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4b71-110">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="b4b71-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4b71-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="b4b71-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4b71-112">Methods</span></span>
|<span data-ttu-id="b4b71-113">Método</span><span class="sxs-lookup"><span data-stu-id="b4b71-113">Method</span></span>|<span data-ttu-id="b4b71-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4b71-114">Return Type</span></span>|<span data-ttu-id="b4b71-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4b71-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4b71-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="b4b71-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="b4b71-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="b4b71-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="b4b71-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4b71-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="b4b71-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="b4b71-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b4b71-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4b71-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b4b71-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="b4b71-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b4b71-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4b71-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b4b71-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="b4b71-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b4b71-126">None</span></span>|<span data-ttu-id="b4b71-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4b71-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="b4b71-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="b4b71-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b4b71-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="b4b71-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b4b71-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b4b71-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4b71-131">Properties</span></span>
|<span data-ttu-id="b4b71-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4b71-132">Property</span></span>|<span data-ttu-id="b4b71-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4b71-133">Type</span></span>|<span data-ttu-id="b4b71-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4b71-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4b71-135">id</span><span class="sxs-lookup"><span data-stu-id="b4b71-135">id</span></span>|<span data-ttu-id="b4b71-136">String</span><span class="sxs-lookup"><span data-stu-id="b4b71-136">String</span></span>|<span data-ttu-id="b4b71-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4b71-137">Unique identifier for the device category.</span></span> <span data-ttu-id="b4b71-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4b71-138">Read-only.</span></span>|
|<span data-ttu-id="b4b71-139">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b4b71-139">**Onboarding**</span></span>|
|<span data-ttu-id="b4b71-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b4b71-140">displayName</span></span>|<span data-ttu-id="b4b71-141">String</span><span class="sxs-lookup"><span data-stu-id="b4b71-141">String</span></span>|<span data-ttu-id="b4b71-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4b71-142">Display name for the device category.</span></span>|
|<span data-ttu-id="b4b71-143">description</span><span class="sxs-lookup"><span data-stu-id="b4b71-143">description</span></span>|<span data-ttu-id="b4b71-144">String</span><span class="sxs-lookup"><span data-stu-id="b4b71-144">String</span></span>|<span data-ttu-id="b4b71-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4b71-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4b71-146">Relações</span><span class="sxs-lookup"><span data-stu-id="b4b71-146">Relationships</span></span>
<span data-ttu-id="b4b71-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4b71-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4b71-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4b71-148">JSON Representation</span></span>
<span data-ttu-id="b4b71-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4b71-149">Here is a JSON representation of the resource.</span></span>
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




