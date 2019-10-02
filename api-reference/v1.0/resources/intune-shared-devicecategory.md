---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 012d473e918160617e016733091e1b2c6931a495
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356097"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="8eacf-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8eacf-104">deviceCategory resource type</span></span>

> <span data-ttu-id="8eacf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eacf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eacf-106">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8eacf-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="8eacf-107">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="8eacf-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="8eacf-108">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eacf-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="8eacf-109">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eacf-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="8eacf-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="8eacf-110">Methods</span></span>
|<span data-ttu-id="8eacf-111">Método</span><span class="sxs-lookup"><span data-stu-id="8eacf-111">Method</span></span>|<span data-ttu-id="8eacf-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8eacf-112">Return Type</span></span>|<span data-ttu-id="8eacf-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eacf-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eacf-114">[Listar deviceCategories](../api/intune-shared-devicecategory-list.md) coleção</span><span class="sxs-lookup"><span data-stu-id="8eacf-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="8eacf-115">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8eacf-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="8eacf-116">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8eacf-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="8eacf-117">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8eacf-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="8eacf-118">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8eacf-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="8eacf-119">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8eacf-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="8eacf-120">[Exclua deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="8eacf-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="8eacf-121">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8eacf-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="8eacf-122">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8eacf-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8eacf-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eacf-123">Properties</span></span>
|<span data-ttu-id="8eacf-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eacf-124">Property</span></span>|<span data-ttu-id="8eacf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eacf-125">Type</span></span>|<span data-ttu-id="8eacf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eacf-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eacf-127">id</span><span class="sxs-lookup"><span data-stu-id="8eacf-127">id</span></span>|<span data-ttu-id="8eacf-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eacf-128">String</span></span>|<span data-ttu-id="8eacf-129">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eacf-129">Unique identifier for the device category.</span></span> <span data-ttu-id="8eacf-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8eacf-130">Read-only.</span></span>|
|<span data-ttu-id="8eacf-131">**Integração**</span><span class="sxs-lookup"><span data-stu-id="8eacf-131">**Onboarding**</span></span>|
|<span data-ttu-id="8eacf-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8eacf-132">displayName</span></span>|<span data-ttu-id="8eacf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eacf-133">String</span></span>|<span data-ttu-id="8eacf-134">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eacf-134">Display name for the device category.</span></span>|
|<span data-ttu-id="8eacf-135">descrição</span><span class="sxs-lookup"><span data-stu-id="8eacf-135">description</span></span>|<span data-ttu-id="8eacf-136">String</span><span class="sxs-lookup"><span data-stu-id="8eacf-136">String</span></span>|<span data-ttu-id="8eacf-137">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eacf-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eacf-138">Relações</span><span class="sxs-lookup"><span data-stu-id="8eacf-138">Relationships</span></span>
<span data-ttu-id="8eacf-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8eacf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eacf-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eacf-140">JSON Representation</span></span>
<span data-ttu-id="8eacf-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eacf-141">Here is a JSON representation of the resource.</span></span>
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




