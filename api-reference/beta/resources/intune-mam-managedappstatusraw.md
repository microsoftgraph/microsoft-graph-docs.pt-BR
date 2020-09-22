---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: afd376bf220c7de53301186cb47e40641ffbdb81
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030154"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="939c5-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="939c5-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="939c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="939c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="939c5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="939c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="939c5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="939c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="939c5-107">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="939c5-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="939c5-108">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="939c5-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="939c5-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="939c5-109">Methods</span></span>
|<span data-ttu-id="939c5-110">Método</span><span class="sxs-lookup"><span data-stu-id="939c5-110">Method</span></span>|<span data-ttu-id="939c5-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="939c5-111">Return Type</span></span>|<span data-ttu-id="939c5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="939c5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="939c5-113">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="939c5-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="939c5-114">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="939c5-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="939c5-115">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="939c5-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="939c5-116">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="939c5-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="939c5-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="939c5-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="939c5-118">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="939c5-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="939c5-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="939c5-119">Properties</span></span>
|<span data-ttu-id="939c5-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="939c5-120">Property</span></span>|<span data-ttu-id="939c5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="939c5-121">Type</span></span>|<span data-ttu-id="939c5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="939c5-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="939c5-123">displayName</span><span class="sxs-lookup"><span data-stu-id="939c5-123">displayName</span></span>|<span data-ttu-id="939c5-124">String</span><span class="sxs-lookup"><span data-stu-id="939c5-124">String</span></span>|<span data-ttu-id="939c5-125">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="939c5-125">Friendly name of the status report.</span></span> <span data-ttu-id="939c5-126">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="939c5-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="939c5-127">id</span><span class="sxs-lookup"><span data-stu-id="939c5-127">id</span></span>|<span data-ttu-id="939c5-128">String</span><span class="sxs-lookup"><span data-stu-id="939c5-128">String</span></span>|<span data-ttu-id="939c5-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="939c5-129">Key of the entity.</span></span> <span data-ttu-id="939c5-130">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="939c5-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="939c5-131">version</span><span class="sxs-lookup"><span data-stu-id="939c5-131">version</span></span>|<span data-ttu-id="939c5-132">String</span><span class="sxs-lookup"><span data-stu-id="939c5-132">String</span></span>|<span data-ttu-id="939c5-133">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="939c5-133">Version of the entity.</span></span> <span data-ttu-id="939c5-134">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="939c5-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="939c5-135">content</span><span class="sxs-lookup"><span data-stu-id="939c5-135">content</span></span>|[<span data-ttu-id="939c5-136">Json</span><span class="sxs-lookup"><span data-stu-id="939c5-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="939c5-137">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="939c5-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="939c5-138">Relações</span><span class="sxs-lookup"><span data-stu-id="939c5-138">Relationships</span></span>
<span data-ttu-id="939c5-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="939c5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="939c5-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="939c5-140">JSON Representation</span></span>
<span data-ttu-id="939c5-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="939c5-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```






