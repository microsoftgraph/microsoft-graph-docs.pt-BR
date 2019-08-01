---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b21c15784409d9d7c373c954faecbc23426041b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037874"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="1af0b-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1af0b-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="1af0b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1af0b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1af0b-105">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="1af0b-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="1af0b-106">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1af0b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1af0b-107">Methods</span></span>
|<span data-ttu-id="1af0b-108">Método</span><span class="sxs-lookup"><span data-stu-id="1af0b-108">Method</span></span>|<span data-ttu-id="1af0b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1af0b-109">Return Type</span></span>|<span data-ttu-id="1af0b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1af0b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1af0b-111">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="1af0b-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="1af0b-112">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="1af0b-113">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="1af0b-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="1af0b-114">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1af0b-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="1af0b-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1af0b-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="1af0b-116">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="1af0b-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1af0b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1af0b-117">Properties</span></span>
|<span data-ttu-id="1af0b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1af0b-118">Property</span></span>|<span data-ttu-id="1af0b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1af0b-119">Type</span></span>|<span data-ttu-id="1af0b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1af0b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1af0b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1af0b-121">displayName</span></span>|<span data-ttu-id="1af0b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1af0b-122">String</span></span>|<span data-ttu-id="1af0b-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="1af0b-123">Friendly name of the status report.</span></span> <span data-ttu-id="1af0b-124">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1af0b-125">id</span><span class="sxs-lookup"><span data-stu-id="1af0b-125">id</span></span>|<span data-ttu-id="1af0b-126">String</span><span class="sxs-lookup"><span data-stu-id="1af0b-126">String</span></span>|<span data-ttu-id="1af0b-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1af0b-127">Key of the entity.</span></span> <span data-ttu-id="1af0b-128">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1af0b-129">version</span><span class="sxs-lookup"><span data-stu-id="1af0b-129">version</span></span>|<span data-ttu-id="1af0b-130">String</span><span class="sxs-lookup"><span data-stu-id="1af0b-130">String</span></span>|<span data-ttu-id="1af0b-131">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1af0b-131">Version of the entity.</span></span> <span data-ttu-id="1af0b-132">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1af0b-133">content</span><span class="sxs-lookup"><span data-stu-id="1af0b-133">content</span></span>|[<span data-ttu-id="1af0b-134">Json</span><span class="sxs-lookup"><span data-stu-id="1af0b-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="1af0b-135">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="1af0b-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1af0b-136">Relações</span><span class="sxs-lookup"><span data-stu-id="1af0b-136">Relationships</span></span>
<span data-ttu-id="1af0b-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1af0b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1af0b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1af0b-138">JSON Representation</span></span>
<span data-ttu-id="1af0b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1af0b-139">Here is a JSON representation of the resource.</span></span>
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



