---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2c19d0e54383c96d7d5ec55e347f116ddfd4ef1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988237"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="9008d-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9008d-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="9008d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9008d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9008d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9008d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9008d-106">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="9008d-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="9008d-107">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9008d-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9008d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9008d-108">Methods</span></span>
|<span data-ttu-id="9008d-109">Método</span><span class="sxs-lookup"><span data-stu-id="9008d-109">Method</span></span>|<span data-ttu-id="9008d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9008d-110">Return Type</span></span>|<span data-ttu-id="9008d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9008d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9008d-112">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="9008d-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="9008d-113">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="9008d-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="9008d-114">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9008d-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="9008d-115">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9008d-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="9008d-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9008d-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="9008d-117">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9008d-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9008d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9008d-118">Properties</span></span>
|<span data-ttu-id="9008d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9008d-119">Property</span></span>|<span data-ttu-id="9008d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9008d-120">Type</span></span>|<span data-ttu-id="9008d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9008d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9008d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="9008d-122">displayName</span></span>|<span data-ttu-id="9008d-123">String</span><span class="sxs-lookup"><span data-stu-id="9008d-123">String</span></span>|<span data-ttu-id="9008d-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="9008d-124">Friendly name of the status report.</span></span> <span data-ttu-id="9008d-125">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9008d-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9008d-126">id</span><span class="sxs-lookup"><span data-stu-id="9008d-126">id</span></span>|<span data-ttu-id="9008d-127">String</span><span class="sxs-lookup"><span data-stu-id="9008d-127">String</span></span>|<span data-ttu-id="9008d-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9008d-128">Key of the entity.</span></span> <span data-ttu-id="9008d-129">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9008d-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9008d-130">version</span><span class="sxs-lookup"><span data-stu-id="9008d-130">version</span></span>|<span data-ttu-id="9008d-131">String</span><span class="sxs-lookup"><span data-stu-id="9008d-131">String</span></span>|<span data-ttu-id="9008d-132">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="9008d-132">Version of the entity.</span></span> <span data-ttu-id="9008d-133">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9008d-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9008d-134">content</span><span class="sxs-lookup"><span data-stu-id="9008d-134">content</span></span>|[<span data-ttu-id="9008d-135">Json</span><span class="sxs-lookup"><span data-stu-id="9008d-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="9008d-136">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="9008d-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9008d-137">Relações</span><span class="sxs-lookup"><span data-stu-id="9008d-137">Relationships</span></span>
<span data-ttu-id="9008d-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9008d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9008d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9008d-139">JSON Representation</span></span>
<span data-ttu-id="9008d-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9008d-140">Here is a JSON representation of the resource.</span></span>
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









