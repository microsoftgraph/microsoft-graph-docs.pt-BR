---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f52c90a7e03ceb2463be3589e60694251d002c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525240"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="f6fe2-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f6fe2-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="f6fe2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f6fe2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6fe2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6fe2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6fe2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6fe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6fe2-107">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="f6fe2-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="f6fe2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f6fe2-108">Methods</span></span>
|<span data-ttu-id="f6fe2-109">Método</span><span class="sxs-lookup"><span data-stu-id="f6fe2-109">Method</span></span>|<span data-ttu-id="f6fe2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6fe2-110">Return Type</span></span>|<span data-ttu-id="f6fe2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6fe2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6fe2-112">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="f6fe2-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="f6fe2-113">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f6fe2-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="f6fe2-114">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="f6fe2-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="f6fe2-115">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f6fe2-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="f6fe2-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="f6fe2-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="f6fe2-117">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="f6fe2-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6fe2-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6fe2-118">Properties</span></span>
|<span data-ttu-id="f6fe2-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6fe2-119">Property</span></span>|<span data-ttu-id="f6fe2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6fe2-120">Type</span></span>|<span data-ttu-id="f6fe2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6fe2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6fe2-122">id</span><span class="sxs-lookup"><span data-stu-id="f6fe2-122">id</span></span>|<span data-ttu-id="f6fe2-123">String</span><span class="sxs-lookup"><span data-stu-id="f6fe2-123">String</span></span>|<span data-ttu-id="f6fe2-124">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="f6fe2-124">The setting instance ID</span></span>|
|<span data-ttu-id="f6fe2-125">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="f6fe2-125">definitionId</span></span>|<span data-ttu-id="f6fe2-126">String</span><span class="sxs-lookup"><span data-stu-id="f6fe2-126">String</span></span>|<span data-ttu-id="f6fe2-127">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="f6fe2-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="f6fe2-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="f6fe2-128">valueJson</span></span>|<span data-ttu-id="f6fe2-129">String</span><span class="sxs-lookup"><span data-stu-id="f6fe2-129">String</span></span>|<span data-ttu-id="f6fe2-130">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="f6fe2-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6fe2-131">Relações</span><span class="sxs-lookup"><span data-stu-id="f6fe2-131">Relationships</span></span>
<span data-ttu-id="f6fe2-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6fe2-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6fe2-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6fe2-133">JSON Representation</span></span>
<span data-ttu-id="f6fe2-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6fe2-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



