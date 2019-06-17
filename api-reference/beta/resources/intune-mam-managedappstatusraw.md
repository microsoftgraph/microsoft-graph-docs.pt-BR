---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12d451a87012da930bb7330cd8eb63ecaa3fec1f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994647"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="80e93-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="80e93-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="80e93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80e93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80e93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80e93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80e93-106">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="80e93-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="80e93-107">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="80e93-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="80e93-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="80e93-108">Methods</span></span>
|<span data-ttu-id="80e93-109">Método</span><span class="sxs-lookup"><span data-stu-id="80e93-109">Method</span></span>|<span data-ttu-id="80e93-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80e93-110">Return Type</span></span>|<span data-ttu-id="80e93-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80e93-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80e93-112">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="80e93-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="80e93-113">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="80e93-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="80e93-114">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="80e93-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="80e93-115">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="80e93-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="80e93-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="80e93-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="80e93-117">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="80e93-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80e93-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80e93-118">Properties</span></span>
|<span data-ttu-id="80e93-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80e93-119">Property</span></span>|<span data-ttu-id="80e93-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="80e93-120">Type</span></span>|<span data-ttu-id="80e93-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="80e93-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e93-122">displayName</span><span class="sxs-lookup"><span data-stu-id="80e93-122">displayName</span></span>|<span data-ttu-id="80e93-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80e93-123">String</span></span>|<span data-ttu-id="80e93-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="80e93-124">Friendly name of the status report.</span></span> <span data-ttu-id="80e93-125">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="80e93-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="80e93-126">id</span><span class="sxs-lookup"><span data-stu-id="80e93-126">id</span></span>|<span data-ttu-id="80e93-127">String</span><span class="sxs-lookup"><span data-stu-id="80e93-127">String</span></span>|<span data-ttu-id="80e93-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80e93-128">Key of the entity.</span></span> <span data-ttu-id="80e93-129">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="80e93-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="80e93-130">version</span><span class="sxs-lookup"><span data-stu-id="80e93-130">version</span></span>|<span data-ttu-id="80e93-131">String</span><span class="sxs-lookup"><span data-stu-id="80e93-131">String</span></span>|<span data-ttu-id="80e93-132">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="80e93-132">Version of the entity.</span></span> <span data-ttu-id="80e93-133">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="80e93-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="80e93-134">content</span><span class="sxs-lookup"><span data-stu-id="80e93-134">content</span></span>|[<span data-ttu-id="80e93-135">Json</span><span class="sxs-lookup"><span data-stu-id="80e93-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="80e93-136">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="80e93-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80e93-137">Relações</span><span class="sxs-lookup"><span data-stu-id="80e93-137">Relationships</span></span>
<span data-ttu-id="80e93-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80e93-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80e93-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80e93-139">JSON Representation</span></span>
<span data-ttu-id="80e93-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80e93-140">Here is a JSON representation of the resource.</span></span>
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





