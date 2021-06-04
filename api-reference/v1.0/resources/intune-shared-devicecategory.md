---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732224"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="43b07-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="43b07-104">deviceCategory resource type</span></span>

<span data-ttu-id="43b07-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b07-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43b07-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43b07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b07-107">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="43b07-107">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="43b07-108">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="43b07-108">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="43b07-109">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43b07-109">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="43b07-110">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43b07-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="43b07-111">Methods</span><span class="sxs-lookup"><span data-stu-id="43b07-111">Methods</span></span>
|<span data-ttu-id="43b07-112">Método</span><span class="sxs-lookup"><span data-stu-id="43b07-112">Method</span></span>|<span data-ttu-id="43b07-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43b07-113">Return Type</span></span>|<span data-ttu-id="43b07-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="43b07-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b07-115">[Listar coleção deviceCategories](../api/intune-shared-devicecategory-list.md)</span><span class="sxs-lookup"><span data-stu-id="43b07-115">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="43b07-116">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="43b07-116">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="43b07-117">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="43b07-117">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="43b07-118">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="43b07-118">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="43b07-119">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="43b07-119">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="43b07-120">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="43b07-120">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="43b07-121">[Excluir deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="43b07-121">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="43b07-122">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="43b07-122">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="43b07-123">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="43b07-123">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43b07-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43b07-124">Properties</span></span>
|<span data-ttu-id="43b07-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43b07-125">Property</span></span>|<span data-ttu-id="43b07-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="43b07-126">Type</span></span>|<span data-ttu-id="43b07-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="43b07-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b07-128">id</span><span class="sxs-lookup"><span data-stu-id="43b07-128">id</span></span>|<span data-ttu-id="43b07-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43b07-129">String</span></span>|<span data-ttu-id="43b07-130">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43b07-130">Unique identifier for the device category.</span></span> <span data-ttu-id="43b07-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43b07-131">Read-only.</span></span>|
|<span data-ttu-id="43b07-132">**Integração**</span><span class="sxs-lookup"><span data-stu-id="43b07-132">**Onboarding**</span></span>|
|<span data-ttu-id="43b07-133">displayName</span><span class="sxs-lookup"><span data-stu-id="43b07-133">displayName</span></span>|<span data-ttu-id="43b07-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43b07-134">String</span></span>|<span data-ttu-id="43b07-135">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43b07-135">Display name for the device category.</span></span>|
|<span data-ttu-id="43b07-136">descrição</span><span class="sxs-lookup"><span data-stu-id="43b07-136">description</span></span>|<span data-ttu-id="43b07-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43b07-137">String</span></span>|<span data-ttu-id="43b07-138">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43b07-138">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43b07-139">Relações</span><span class="sxs-lookup"><span data-stu-id="43b07-139">Relationships</span></span>
<span data-ttu-id="43b07-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="43b07-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43b07-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43b07-141">JSON Representation</span></span>
<span data-ttu-id="43b07-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43b07-142">Here is a JSON representation of the resource.</span></span>
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









