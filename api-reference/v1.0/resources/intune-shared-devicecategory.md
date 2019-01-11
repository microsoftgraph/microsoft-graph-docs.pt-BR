---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80f8f1f36198ecfab1021e30cb2f28fa4377852c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810833"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="2c985-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2c985-104">deviceCategory resource type</span></span>

> <span data-ttu-id="2c985-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2c985-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c985-106">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2c985-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="2c985-107">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="2c985-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="2c985-108">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c985-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="2c985-109">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c985-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="2c985-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c985-110">Methods</span></span>
|<span data-ttu-id="2c985-111">Método</span><span class="sxs-lookup"><span data-stu-id="2c985-111">Method</span></span>|<span data-ttu-id="2c985-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c985-112">Return Type</span></span>|<span data-ttu-id="2c985-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c985-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c985-114">Coleção da [lista deviceCategories](../api/intune-shared-devicecategory-list.md)</span><span class="sxs-lookup"><span data-stu-id="2c985-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="2c985-115">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2c985-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="2c985-116">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2c985-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="2c985-117">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2c985-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="2c985-118">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2c985-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="2c985-119">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2c985-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="2c985-120">[Excluir deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="2c985-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="2c985-121">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2c985-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="2c985-122">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2c985-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c985-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c985-123">Properties</span></span>
|<span data-ttu-id="2c985-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c985-124">Property</span></span>|<span data-ttu-id="2c985-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c985-125">Type</span></span>|<span data-ttu-id="2c985-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c985-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c985-127">id</span><span class="sxs-lookup"><span data-stu-id="2c985-127">id</span></span>|<span data-ttu-id="2c985-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c985-128">String</span></span>|<span data-ttu-id="2c985-129">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c985-129">Unique identifier for the device category.</span></span> <span data-ttu-id="2c985-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c985-130">Read-only.</span></span>|
|<span data-ttu-id="2c985-131">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="2c985-131">**Onboarding**</span></span>|
|<span data-ttu-id="2c985-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2c985-132">displayName</span></span>|<span data-ttu-id="2c985-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c985-133">String</span></span>|<span data-ttu-id="2c985-134">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c985-134">Display name for the device category.</span></span>|
|<span data-ttu-id="2c985-135">description</span><span class="sxs-lookup"><span data-stu-id="2c985-135">description</span></span>|<span data-ttu-id="2c985-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c985-136">String</span></span>|<span data-ttu-id="2c985-137">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c985-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c985-138">Relações</span><span class="sxs-lookup"><span data-stu-id="2c985-138">Relationships</span></span>
<span data-ttu-id="2c985-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c985-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c985-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c985-140">JSON Representation</span></span>
<span data-ttu-id="2c985-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c985-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



