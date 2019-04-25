---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75fb11ef3b734e6d5d0490be1abc3c5399433a70
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525317"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="462d5-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-104">deviceCategory resource type</span></span>

> <span data-ttu-id="462d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="462d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="462d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="462d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="462d5-107">As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="462d5-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="462d5-108">Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="462d5-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="462d5-109">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="462d5-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="462d5-110">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="462d5-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="462d5-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="462d5-111">Methods</span></span>
|<span data-ttu-id="462d5-112">Método</span><span class="sxs-lookup"><span data-stu-id="462d5-112">Method</span></span>|<span data-ttu-id="462d5-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="462d5-113">Return Type</span></span>|<span data-ttu-id="462d5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="462d5-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="462d5-115">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="462d5-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="462d5-116">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="462d5-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="462d5-117">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="462d5-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="462d5-118">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="462d5-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="462d5-120">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="462d5-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="462d5-121">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="462d5-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="462d5-123">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="462d5-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="462d5-124">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="462d5-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="462d5-125">None</span></span>|<span data-ttu-id="462d5-126">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="462d5-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="462d5-127">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="462d5-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="462d5-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="462d5-129">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="462d5-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="462d5-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="462d5-130">Properties</span></span>
|<span data-ttu-id="462d5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="462d5-131">Property</span></span>|<span data-ttu-id="462d5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="462d5-132">Type</span></span>|<span data-ttu-id="462d5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="462d5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="462d5-134">id</span><span class="sxs-lookup"><span data-stu-id="462d5-134">id</span></span>|<span data-ttu-id="462d5-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="462d5-135">String</span></span>|<span data-ttu-id="462d5-136">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="462d5-136">Unique identifier for the device category.</span></span> <span data-ttu-id="462d5-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="462d5-137">Read-only.</span></span>|
|<span data-ttu-id="462d5-138">**Integração**</span><span class="sxs-lookup"><span data-stu-id="462d5-138">**Onboarding**</span></span>|
|<span data-ttu-id="462d5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="462d5-139">displayName</span></span>|<span data-ttu-id="462d5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="462d5-140">String</span></span>|<span data-ttu-id="462d5-141">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="462d5-141">Display name for the device category.</span></span>|
|<span data-ttu-id="462d5-142">description</span><span class="sxs-lookup"><span data-stu-id="462d5-142">description</span></span>|<span data-ttu-id="462d5-143">String</span><span class="sxs-lookup"><span data-stu-id="462d5-143">String</span></span>|<span data-ttu-id="462d5-144">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="462d5-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="462d5-145">Relações</span><span class="sxs-lookup"><span data-stu-id="462d5-145">Relationships</span></span>
<span data-ttu-id="462d5-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="462d5-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="462d5-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="462d5-147">JSON Representation</span></span>
<span data-ttu-id="462d5-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="462d5-148">Here is a JSON representation of the resource.</span></span>
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



