---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 529b6b654c176b5062910a2cea0d03622faa78c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940677"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="9e5df-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9e5df-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="9e5df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e5df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e5df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e5df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e5df-106">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="9e5df-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="9e5df-107">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9e5df-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9e5df-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e5df-108">Methods</span></span>
|<span data-ttu-id="9e5df-109">Método</span><span class="sxs-lookup"><span data-stu-id="9e5df-109">Method</span></span>|<span data-ttu-id="9e5df-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e5df-110">Return Type</span></span>|<span data-ttu-id="9e5df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5df-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e5df-112">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="9e5df-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="9e5df-113">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="9e5df-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="9e5df-114">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9e5df-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="9e5df-115">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9e5df-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="9e5df-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="9e5df-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="9e5df-117">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="9e5df-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e5df-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e5df-118">Properties</span></span>
|<span data-ttu-id="9e5df-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e5df-119">Property</span></span>|<span data-ttu-id="9e5df-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e5df-120">Type</span></span>|<span data-ttu-id="9e5df-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e5df-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e5df-122">displayName</span><span class="sxs-lookup"><span data-stu-id="9e5df-122">displayName</span></span>|<span data-ttu-id="9e5df-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5df-123">String</span></span>|<span data-ttu-id="9e5df-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="9e5df-124">Friendly name of the status report.</span></span> <span data-ttu-id="9e5df-125">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9e5df-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9e5df-126">id</span><span class="sxs-lookup"><span data-stu-id="9e5df-126">id</span></span>|<span data-ttu-id="9e5df-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e5df-127">String</span></span>|<span data-ttu-id="9e5df-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e5df-128">Key of the entity.</span></span> <span data-ttu-id="9e5df-129">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9e5df-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9e5df-130">version</span><span class="sxs-lookup"><span data-stu-id="9e5df-130">version</span></span>|<span data-ttu-id="9e5df-131">String</span><span class="sxs-lookup"><span data-stu-id="9e5df-131">String</span></span>|<span data-ttu-id="9e5df-132">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e5df-132">Version of the entity.</span></span> <span data-ttu-id="9e5df-133">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9e5df-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="9e5df-134">content</span><span class="sxs-lookup"><span data-stu-id="9e5df-134">content</span></span>|[<span data-ttu-id="9e5df-135">Json</span><span class="sxs-lookup"><span data-stu-id="9e5df-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="9e5df-136">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="9e5df-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e5df-137">Relações</span><span class="sxs-lookup"><span data-stu-id="9e5df-137">Relationships</span></span>
<span data-ttu-id="9e5df-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e5df-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e5df-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e5df-139">JSON Representation</span></span>
<span data-ttu-id="9e5df-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e5df-140">Here is a JSON representation of the resource.</span></span>
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




