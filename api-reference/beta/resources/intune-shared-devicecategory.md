---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
ms.openlocfilehash: 4416dc1557cdae38313aa8aa1e73cda82d764e9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359539"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="5831d-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-104">deviceCategory resource type</span></span>

> <span data-ttu-id="5831d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5831d-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5831d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5831d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5831d-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5831d-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5831d-108">Categorias de dispositivos fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5831d-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="5831d-109">Usando categorias de dispositivo, administradores de empresa podem definir categorias exclusivas que faz sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="5831d-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="5831d-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5831d-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="5831d-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5831d-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="5831d-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="5831d-112">Methods</span></span>
|<span data-ttu-id="5831d-113">Método</span><span class="sxs-lookup"><span data-stu-id="5831d-113">Method</span></span>|<span data-ttu-id="5831d-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5831d-114">Return Type</span></span>|<span data-ttu-id="5831d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="5831d-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5831d-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="5831d-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="5831d-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="5831d-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="5831d-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5831d-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="5831d-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="5831d-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5831d-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5831d-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="5831d-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="5831d-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5831d-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5831d-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="5831d-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="5831d-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5831d-126">None</span></span>|<span data-ttu-id="5831d-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5831d-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="5831d-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="5831d-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5831d-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="5831d-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5831d-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5831d-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5831d-131">Properties</span></span>
|<span data-ttu-id="5831d-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5831d-132">Property</span></span>|<span data-ttu-id="5831d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5831d-133">Type</span></span>|<span data-ttu-id="5831d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5831d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5831d-135">id</span><span class="sxs-lookup"><span data-stu-id="5831d-135">id</span></span>|<span data-ttu-id="5831d-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5831d-136">String</span></span>|<span data-ttu-id="5831d-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5831d-137">Unique identifier for the device category.</span></span> <span data-ttu-id="5831d-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5831d-138">Read-only.</span></span>|
|<span data-ttu-id="5831d-139">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="5831d-139">**Onboarding**</span></span>|
|<span data-ttu-id="5831d-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5831d-140">displayName</span></span>|<span data-ttu-id="5831d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5831d-141">String</span></span>|<span data-ttu-id="5831d-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5831d-142">Display name for the device category.</span></span>|
|<span data-ttu-id="5831d-143">description</span><span class="sxs-lookup"><span data-stu-id="5831d-143">description</span></span>|<span data-ttu-id="5831d-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5831d-144">String</span></span>|<span data-ttu-id="5831d-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5831d-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5831d-146">Relações</span><span class="sxs-lookup"><span data-stu-id="5831d-146">Relationships</span></span>
<span data-ttu-id="5831d-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5831d-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5831d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5831d-148">JSON Representation</span></span>
<span data-ttu-id="5831d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5831d-149">Here is a JSON representation of the resource.</span></span>
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



