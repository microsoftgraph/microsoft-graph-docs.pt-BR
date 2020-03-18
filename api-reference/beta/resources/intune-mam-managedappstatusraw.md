---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 292cd8c17702705774b650c257c4ae9ce1ff0ff3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781415"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="36a70-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="36a70-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="36a70-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36a70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36a70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a70-106">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="36a70-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="36a70-107">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="36a70-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="36a70-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="36a70-108">Methods</span></span>
|<span data-ttu-id="36a70-109">Método</span><span class="sxs-lookup"><span data-stu-id="36a70-109">Method</span></span>|<span data-ttu-id="36a70-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36a70-110">Return Type</span></span>|<span data-ttu-id="36a70-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="36a70-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36a70-112">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="36a70-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="36a70-113">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="36a70-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="36a70-114">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="36a70-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="36a70-115">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="36a70-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="36a70-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="36a70-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="36a70-117">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="36a70-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36a70-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36a70-118">Properties</span></span>
|<span data-ttu-id="36a70-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36a70-119">Property</span></span>|<span data-ttu-id="36a70-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="36a70-120">Type</span></span>|<span data-ttu-id="36a70-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="36a70-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a70-122">displayName</span><span class="sxs-lookup"><span data-stu-id="36a70-122">displayName</span></span>|<span data-ttu-id="36a70-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36a70-123">String</span></span>|<span data-ttu-id="36a70-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="36a70-124">Friendly name of the status report.</span></span> <span data-ttu-id="36a70-125">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="36a70-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="36a70-126">id</span><span class="sxs-lookup"><span data-stu-id="36a70-126">id</span></span>|<span data-ttu-id="36a70-127">String</span><span class="sxs-lookup"><span data-stu-id="36a70-127">String</span></span>|<span data-ttu-id="36a70-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36a70-128">Key of the entity.</span></span> <span data-ttu-id="36a70-129">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="36a70-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="36a70-130">version</span><span class="sxs-lookup"><span data-stu-id="36a70-130">version</span></span>|<span data-ttu-id="36a70-131">String</span><span class="sxs-lookup"><span data-stu-id="36a70-131">String</span></span>|<span data-ttu-id="36a70-132">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="36a70-132">Version of the entity.</span></span> <span data-ttu-id="36a70-133">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="36a70-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="36a70-134">content</span><span class="sxs-lookup"><span data-stu-id="36a70-134">content</span></span>|[<span data-ttu-id="36a70-135">Json</span><span class="sxs-lookup"><span data-stu-id="36a70-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="36a70-136">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="36a70-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36a70-137">Relações</span><span class="sxs-lookup"><span data-stu-id="36a70-137">Relationships</span></span>
<span data-ttu-id="36a70-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36a70-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36a70-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36a70-139">JSON Representation</span></span>
<span data-ttu-id="36a70-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36a70-140">Here is a JSON representation of the resource.</span></span>
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



