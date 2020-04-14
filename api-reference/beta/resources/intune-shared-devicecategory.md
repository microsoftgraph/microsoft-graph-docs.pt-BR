---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0aa67ac9dbe7be255ff1b27013f7e2eeecb7d185
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443629"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="5561a-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-104">deviceCategory resource type</span></span>

<span data-ttu-id="5561a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5561a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5561a-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5561a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5561a-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5561a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5561a-108">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5561a-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="5561a-109">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="5561a-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="5561a-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5561a-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="5561a-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5561a-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="5561a-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="5561a-112">Methods</span></span>
|<span data-ttu-id="5561a-113">Método</span><span class="sxs-lookup"><span data-stu-id="5561a-113">Method</span></span>|<span data-ttu-id="5561a-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5561a-114">Return Type</span></span>|<span data-ttu-id="5561a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="5561a-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5561a-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="5561a-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="5561a-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="5561a-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="5561a-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5561a-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="5561a-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="5561a-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5561a-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5561a-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="5561a-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="5561a-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5561a-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5561a-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="5561a-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="5561a-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5561a-126">None</span></span>|<span data-ttu-id="5561a-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5561a-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="5561a-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="5561a-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5561a-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5561a-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5561a-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5561a-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5561a-131">Properties</span></span>
|<span data-ttu-id="5561a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5561a-132">Property</span></span>|<span data-ttu-id="5561a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5561a-133">Type</span></span>|<span data-ttu-id="5561a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5561a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5561a-135">id</span><span class="sxs-lookup"><span data-stu-id="5561a-135">id</span></span>|<span data-ttu-id="5561a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5561a-136">String</span></span>|<span data-ttu-id="5561a-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5561a-137">Unique identifier for the device category.</span></span> <span data-ttu-id="5561a-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5561a-138">Read-only.</span></span>|
|<span data-ttu-id="5561a-139">**Integração**</span><span class="sxs-lookup"><span data-stu-id="5561a-139">**Onboarding**</span></span>|
|<span data-ttu-id="5561a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5561a-140">displayName</span></span>|<span data-ttu-id="5561a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5561a-141">String</span></span>|<span data-ttu-id="5561a-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5561a-142">Display name for the device category.</span></span>|
|<span data-ttu-id="5561a-143">description</span><span class="sxs-lookup"><span data-stu-id="5561a-143">description</span></span>|<span data-ttu-id="5561a-144">String</span><span class="sxs-lookup"><span data-stu-id="5561a-144">String</span></span>|<span data-ttu-id="5561a-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5561a-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5561a-146">Relações</span><span class="sxs-lookup"><span data-stu-id="5561a-146">Relationships</span></span>
<span data-ttu-id="5561a-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5561a-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5561a-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5561a-148">JSON Representation</span></span>
<span data-ttu-id="5561a-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5561a-149">Here is a JSON representation of the resource.</span></span>
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



