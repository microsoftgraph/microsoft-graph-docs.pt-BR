---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a035fcb23b3137bfe4e278e12d71a754d1e69d05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061179"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="c2f31-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c2f31-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="c2f31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2f31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2f31-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2f31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2f31-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2f31-107">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="c2f31-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="c2f31-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c2f31-108">Methods</span></span>
|<span data-ttu-id="c2f31-109">Método</span><span class="sxs-lookup"><span data-stu-id="c2f31-109">Method</span></span>|<span data-ttu-id="c2f31-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c2f31-110">Return Type</span></span>|<span data-ttu-id="c2f31-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2f31-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2f31-112">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="c2f31-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="c2f31-113">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c2f31-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="c2f31-114">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c2f31-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="c2f31-115">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c2f31-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="c2f31-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="c2f31-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="c2f31-117">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c2f31-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2f31-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2f31-118">Properties</span></span>
|<span data-ttu-id="c2f31-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2f31-119">Property</span></span>|<span data-ttu-id="c2f31-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2f31-120">Type</span></span>|<span data-ttu-id="c2f31-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2f31-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f31-122">id</span><span class="sxs-lookup"><span data-stu-id="c2f31-122">id</span></span>|<span data-ttu-id="c2f31-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2f31-123">String</span></span>|<span data-ttu-id="c2f31-124">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="c2f31-124">The setting instance ID</span></span>|
|<span data-ttu-id="c2f31-125">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="c2f31-125">definitionId</span></span>|<span data-ttu-id="c2f31-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2f31-126">String</span></span>|<span data-ttu-id="c2f31-127">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="c2f31-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="c2f31-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="c2f31-128">valueJson</span></span>|<span data-ttu-id="c2f31-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2f31-129">String</span></span>|<span data-ttu-id="c2f31-130">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="c2f31-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2f31-131">Relações</span><span class="sxs-lookup"><span data-stu-id="c2f31-131">Relationships</span></span>
<span data-ttu-id="c2f31-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2f31-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2f31-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2f31-133">JSON Representation</span></span>
<span data-ttu-id="c2f31-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2f31-134">Here is a JSON representation of the resource.</span></span>
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






