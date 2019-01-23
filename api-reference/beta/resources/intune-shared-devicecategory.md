---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7470f6cf0193474bfaff4f7444ed3df1d9453a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418859"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="fbf8b-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-104">deviceCategory resource type</span></span>

> <span data-ttu-id="fbf8b-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbf8b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbf8b-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbf8b-108">Categorias de dispositivos fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="fbf8b-109">Usando categorias de dispositivo, administradores de empresa podem definir categorias exclusivas que faz sentido para sua empresa.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="fbf8b-110">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="fbf8b-111">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="fbf8b-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbf8b-112">Methods</span></span>
|<span data-ttu-id="fbf8b-113">Método</span><span class="sxs-lookup"><span data-stu-id="fbf8b-113">Method</span></span>|<span data-ttu-id="fbf8b-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbf8b-114">Return Type</span></span>|<span data-ttu-id="fbf8b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf8b-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbf8b-116">Listar deviceCategories</span><span class="sxs-lookup"><span data-stu-id="fbf8b-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="fbf8b-117">Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="fbf8b-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="fbf8b-118">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8b-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="fbf8b-119">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="fbf8b-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="fbf8b-121">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8b-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="fbf8b-122">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="fbf8b-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="fbf8b-124">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8b-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="fbf8b-125">Excluir deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="fbf8b-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fbf8b-126">None</span></span>|<span data-ttu-id="fbf8b-127">Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8b-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="fbf8b-128">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="fbf8b-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fbf8b-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="fbf8b-130">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fbf8b-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbf8b-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbf8b-131">Properties</span></span>
|<span data-ttu-id="fbf8b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbf8b-132">Property</span></span>|<span data-ttu-id="fbf8b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbf8b-133">Type</span></span>|<span data-ttu-id="fbf8b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbf8b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbf8b-135">id</span><span class="sxs-lookup"><span data-stu-id="fbf8b-135">id</span></span>|<span data-ttu-id="fbf8b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8b-136">String</span></span>|<span data-ttu-id="fbf8b-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-137">Unique identifier for the device category.</span></span> <span data-ttu-id="fbf8b-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-138">Read-only.</span></span>|
|<span data-ttu-id="fbf8b-139">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="fbf8b-139">**Onboarding**</span></span>|
|<span data-ttu-id="fbf8b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="fbf8b-140">displayName</span></span>|<span data-ttu-id="fbf8b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8b-141">String</span></span>|<span data-ttu-id="fbf8b-142">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-142">Display name for the device category.</span></span>|
|<span data-ttu-id="fbf8b-143">description</span><span class="sxs-lookup"><span data-stu-id="fbf8b-143">description</span></span>|<span data-ttu-id="fbf8b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbf8b-144">String</span></span>|<span data-ttu-id="fbf8b-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbf8b-146">Relações</span><span class="sxs-lookup"><span data-stu-id="fbf8b-146">Relationships</span></span>
<span data-ttu-id="fbf8b-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbf8b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbf8b-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbf8b-148">JSON Representation</span></span>
<span data-ttu-id="fbf8b-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbf8b-149">Here is a JSON representation of the resource.</span></span>
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



