---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49f97d47b5ff75e927a5637356476392047a2f8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550536"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="31db6-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="31db6-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="31db6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31db6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31db6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31db6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31db6-106">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="31db6-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="31db6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="31db6-107">Methods</span></span>
|<span data-ttu-id="31db6-108">Método</span><span class="sxs-lookup"><span data-stu-id="31db6-108">Method</span></span>|<span data-ttu-id="31db6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="31db6-109">Return Type</span></span>|<span data-ttu-id="31db6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="31db6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31db6-111">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="31db6-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="31db6-112">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="31db6-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="31db6-113">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="31db6-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="31db6-114">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="31db6-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="31db6-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="31db6-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="31db6-116">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="31db6-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31db6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31db6-117">Properties</span></span>
|<span data-ttu-id="31db6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31db6-118">Property</span></span>|<span data-ttu-id="31db6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="31db6-119">Type</span></span>|<span data-ttu-id="31db6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="31db6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31db6-121">id</span><span class="sxs-lookup"><span data-stu-id="31db6-121">id</span></span>|<span data-ttu-id="31db6-122">String</span><span class="sxs-lookup"><span data-stu-id="31db6-122">String</span></span>|<span data-ttu-id="31db6-123">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="31db6-123">The setting instance ID</span></span>|
|<span data-ttu-id="31db6-124">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="31db6-124">definitionId</span></span>|<span data-ttu-id="31db6-125">String</span><span class="sxs-lookup"><span data-stu-id="31db6-125">String</span></span>|<span data-ttu-id="31db6-126">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="31db6-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="31db6-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="31db6-127">valueJson</span></span>|<span data-ttu-id="31db6-128">String</span><span class="sxs-lookup"><span data-stu-id="31db6-128">String</span></span>|<span data-ttu-id="31db6-129">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="31db6-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="31db6-130">Relações</span><span class="sxs-lookup"><span data-stu-id="31db6-130">Relationships</span></span>
<span data-ttu-id="31db6-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31db6-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31db6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31db6-132">JSON Representation</span></span>
<span data-ttu-id="31db6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31db6-133">Here is a JSON representation of the resource.</span></span>
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





