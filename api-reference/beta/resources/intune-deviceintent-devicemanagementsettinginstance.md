---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 628ca393006666f7a655cf45832784e88f2a4d01
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984489"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="0f780-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0f780-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="0f780-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f780-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f780-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f780-106">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="0f780-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="0f780-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f780-107">Methods</span></span>
|<span data-ttu-id="0f780-108">Método</span><span class="sxs-lookup"><span data-stu-id="0f780-108">Method</span></span>|<span data-ttu-id="0f780-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f780-109">Return Type</span></span>|<span data-ttu-id="0f780-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f780-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f780-111">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="0f780-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="0f780-112">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0f780-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="0f780-113">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="0f780-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="0f780-114">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0f780-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="0f780-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0f780-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="0f780-116">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="0f780-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f780-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f780-117">Properties</span></span>
|<span data-ttu-id="0f780-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f780-118">Property</span></span>|<span data-ttu-id="0f780-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f780-119">Type</span></span>|<span data-ttu-id="0f780-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f780-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f780-121">id</span><span class="sxs-lookup"><span data-stu-id="0f780-121">id</span></span>|<span data-ttu-id="0f780-122">String</span><span class="sxs-lookup"><span data-stu-id="0f780-122">String</span></span>|<span data-ttu-id="0f780-123">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="0f780-123">The setting instance ID</span></span>|
|<span data-ttu-id="0f780-124">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="0f780-124">definitionId</span></span>|<span data-ttu-id="0f780-125">String</span><span class="sxs-lookup"><span data-stu-id="0f780-125">String</span></span>|<span data-ttu-id="0f780-126">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="0f780-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="0f780-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="0f780-127">valueJson</span></span>|<span data-ttu-id="0f780-128">String</span><span class="sxs-lookup"><span data-stu-id="0f780-128">String</span></span>|<span data-ttu-id="0f780-129">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="0f780-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f780-130">Relações</span><span class="sxs-lookup"><span data-stu-id="0f780-130">Relationships</span></span>
<span data-ttu-id="0f780-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f780-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f780-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f780-132">JSON Representation</span></span>
<span data-ttu-id="0f780-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f780-133">Here is a JSON representation of the resource.</span></span>
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





