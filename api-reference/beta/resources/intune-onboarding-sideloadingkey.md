---
title: tipo de recurso de sideLoadingKey
description: Entidade SideLoadingKey é necessária para o Windows 8 e 8.1 dispositivos para instalar aplicativos de linha de negócios para um inquilino.
author: tfitzmac
ms.openlocfilehash: 66dc833ab46f8dc1c030a3ef97be78cd73ee3660
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304309"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="6d3d0-103">tipo de recurso de sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="6d3d0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d3d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d3d0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d3d0-107">Entidade SideLoadingKey é necessária para o Windows 8 e 8.1 dispositivos para instalar aplicativos de linha de negócios para um inquilino.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="6d3d0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d3d0-108">Methods</span></span>
|<span data-ttu-id="6d3d0-109">Método</span><span class="sxs-lookup"><span data-stu-id="6d3d0-109">Method</span></span>|<span data-ttu-id="6d3d0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d3d0-110">Return Type</span></span>|<span data-ttu-id="6d3d0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3d0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d3d0-112">Lista sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="6d3d0-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="6d3d0-113">coleção [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="6d3d0-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="6d3d0-114">Lista as propriedades e os relacionamentos dos objetos [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3d0-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="6d3d0-115">Obter sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="6d3d0-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="6d3d0-117">Leia as propriedades e os relacionamentos do objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3d0-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="6d3d0-118">Criar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="6d3d0-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="6d3d0-120">Crie um novo objeto de [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3d0-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="6d3d0-121">Excluir sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="6d3d0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d3d0-122">None</span></span>|<span data-ttu-id="6d3d0-123">Exclui um [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="6d3d0-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="6d3d0-124">Atualizar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="6d3d0-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="6d3d0-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="6d3d0-126">Atualize as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="6d3d0-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d3d0-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d3d0-127">Properties</span></span>
|<span data-ttu-id="6d3d0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d3d0-128">Property</span></span>|<span data-ttu-id="6d3d0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3d0-129">Type</span></span>|<span data-ttu-id="6d3d0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3d0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d3d0-131">id</span><span class="sxs-lookup"><span data-stu-id="6d3d0-131">id</span></span>|<span data-ttu-id="6d3d0-132">String</span><span class="sxs-lookup"><span data-stu-id="6d3d0-132">String</span></span>|<span data-ttu-id="6d3d0-133">Lado carregando o ID exclusivo principal.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="6d3d0-134">valor</span><span class="sxs-lookup"><span data-stu-id="6d3d0-134">value</span></span>|<span data-ttu-id="6d3d0-135">String</span><span class="sxs-lookup"><span data-stu-id="6d3d0-135">String</span></span>|<span data-ttu-id="6d3d0-136">Valor da chave Carregando lado, é 5x5 valor, separados por hiphens.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="6d3d0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6d3d0-137">displayName</span></span>|<span data-ttu-id="6d3d0-138">String</span><span class="sxs-lookup"><span data-stu-id="6d3d0-138">String</span></span>|<span data-ttu-id="6d3d0-139">Carregando da lado chave nome exibido para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="6d3d0-140">description</span><span class="sxs-lookup"><span data-stu-id="6d3d0-140">description</span></span>|<span data-ttu-id="6d3d0-141">String</span><span class="sxs-lookup"><span data-stu-id="6d3d0-141">String</span></span>|<span data-ttu-id="6d3d0-142">Descrição de chave Carregando lado exibida para o ITPro Admins..</span><span class="sxs-lookup"><span data-stu-id="6d3d0-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="6d3d0-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="6d3d0-143">totalActivation</span></span>|<span data-ttu-id="6d3d0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6d3d0-144">Int32</span></span>|<span data-ttu-id="6d3d0-145">Lado Carregando chave Total Activation exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="6d3d0-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d3d0-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="6d3d0-147">String</span><span class="sxs-lookup"><span data-stu-id="6d3d0-147">String</span></span>|<span data-ttu-id="6d3d0-148">Lado Carregando chave última atualizado data exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d3d0-149">Relações</span><span class="sxs-lookup"><span data-stu-id="6d3d0-149">Relationships</span></span>
<span data-ttu-id="6d3d0-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d3d0-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d3d0-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d3d0-151">JSON Representation</span></span>
<span data-ttu-id="6d3d0-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d3d0-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





