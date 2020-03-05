---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cca08ce1f93a36a17f3743d5e93d98b668212c58
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447861"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="d41bb-104">Tipo de recurso deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d41bb-104">deviceCategory resource type</span></span>

<span data-ttu-id="d41bb-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d41bb-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d41bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d41bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41bb-107">Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d41bb-107">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="d41bb-108">Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.</span><span class="sxs-lookup"><span data-stu-id="d41bb-108">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="d41bb-109">Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d41bb-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="d41bb-110">Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d41bb-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="d41bb-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d41bb-111">Methods</span></span>
|<span data-ttu-id="d41bb-112">Método</span><span class="sxs-lookup"><span data-stu-id="d41bb-112">Method</span></span>|<span data-ttu-id="d41bb-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d41bb-113">Return Type</span></span>|<span data-ttu-id="d41bb-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d41bb-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41bb-115">[Listar deviceCategories](../api/intune-shared-devicecategory-list.md) coleção</span><span class="sxs-lookup"><span data-stu-id="d41bb-115">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="d41bb-116">Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d41bb-116">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="d41bb-117">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d41bb-117">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="d41bb-118">Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d41bb-118">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="d41bb-119">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d41bb-119">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="d41bb-120">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d41bb-120">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="d41bb-121">[Exclua deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="d41bb-121">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="d41bb-122">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d41bb-122">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="d41bb-123">Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d41bb-123">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d41bb-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d41bb-124">Properties</span></span>
|<span data-ttu-id="d41bb-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d41bb-125">Property</span></span>|<span data-ttu-id="d41bb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d41bb-126">Type</span></span>|<span data-ttu-id="d41bb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d41bb-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41bb-128">id</span><span class="sxs-lookup"><span data-stu-id="d41bb-128">id</span></span>|<span data-ttu-id="d41bb-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d41bb-129">String</span></span>|<span data-ttu-id="d41bb-130">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d41bb-130">Unique identifier for the device category.</span></span> <span data-ttu-id="d41bb-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d41bb-131">Read-only.</span></span>|
|<span data-ttu-id="d41bb-132">**Integração**</span><span class="sxs-lookup"><span data-stu-id="d41bb-132">**Onboarding**</span></span>|
|<span data-ttu-id="d41bb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d41bb-133">displayName</span></span>|<span data-ttu-id="d41bb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d41bb-134">String</span></span>|<span data-ttu-id="d41bb-135">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d41bb-135">Display name for the device category.</span></span>|
|<span data-ttu-id="d41bb-136">description</span><span class="sxs-lookup"><span data-stu-id="d41bb-136">description</span></span>|<span data-ttu-id="d41bb-137">String</span><span class="sxs-lookup"><span data-stu-id="d41bb-137">String</span></span>|<span data-ttu-id="d41bb-138">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d41bb-138">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41bb-139">Relações</span><span class="sxs-lookup"><span data-stu-id="d41bb-139">Relationships</span></span>
<span data-ttu-id="d41bb-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d41bb-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d41bb-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d41bb-141">JSON Representation</span></span>
<span data-ttu-id="d41bb-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d41bb-142">Here is a JSON representation of the resource.</span></span>
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




