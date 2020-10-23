---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 039a3f49c877a9c54d11a88351fa6e5fd6c349d4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702345"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="0f8ef-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0f8ef-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="0f8ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f8ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f8ef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f8ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f8ef-107">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="0f8ef-108">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ef-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0f8ef-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f8ef-109">Methods</span></span>
|<span data-ttu-id="0f8ef-110">Método</span><span class="sxs-lookup"><span data-stu-id="0f8ef-110">Method</span></span>|<span data-ttu-id="0f8ef-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f8ef-111">Return Type</span></span>|<span data-ttu-id="0f8ef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f8ef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f8ef-113">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="0f8ef-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="0f8ef-114">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ef-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="0f8ef-115">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="0f8ef-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="0f8ef-116">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0f8ef-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="0f8ef-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0f8ef-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="0f8ef-118">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="0f8ef-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f8ef-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f8ef-119">Properties</span></span>
|<span data-ttu-id="0f8ef-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f8ef-120">Property</span></span>|<span data-ttu-id="0f8ef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f8ef-121">Type</span></span>|<span data-ttu-id="0f8ef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f8ef-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f8ef-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0f8ef-123">displayName</span></span>|<span data-ttu-id="0f8ef-124">String</span><span class="sxs-lookup"><span data-stu-id="0f8ef-124">String</span></span>|<span data-ttu-id="0f8ef-125">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-125">Friendly name of the status report.</span></span> <span data-ttu-id="0f8ef-126">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ef-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f8ef-127">id</span><span class="sxs-lookup"><span data-stu-id="0f8ef-127">id</span></span>|<span data-ttu-id="0f8ef-128">String</span><span class="sxs-lookup"><span data-stu-id="0f8ef-128">String</span></span>|<span data-ttu-id="0f8ef-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-129">Key of the entity.</span></span> <span data-ttu-id="0f8ef-130">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ef-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f8ef-131">version</span><span class="sxs-lookup"><span data-stu-id="0f8ef-131">version</span></span>|<span data-ttu-id="0f8ef-132">String</span><span class="sxs-lookup"><span data-stu-id="0f8ef-132">String</span></span>|<span data-ttu-id="0f8ef-133">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-133">Version of the entity.</span></span> <span data-ttu-id="0f8ef-134">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ef-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f8ef-135">content</span><span class="sxs-lookup"><span data-stu-id="0f8ef-135">content</span></span>|[<span data-ttu-id="0f8ef-136">Json</span><span class="sxs-lookup"><span data-stu-id="0f8ef-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="0f8ef-137">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f8ef-138">Relações</span><span class="sxs-lookup"><span data-stu-id="0f8ef-138">Relationships</span></span>
<span data-ttu-id="0f8ef-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f8ef-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f8ef-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f8ef-140">JSON Representation</span></span>
<span data-ttu-id="0f8ef-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f8ef-141">Here is a JSON representation of the resource.</span></span>
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





