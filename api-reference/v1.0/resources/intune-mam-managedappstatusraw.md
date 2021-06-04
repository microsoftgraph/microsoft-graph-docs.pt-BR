---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d29ec2d96d38c6bc1f2fccf5fb5b36e16e1c5be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752767"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="5b135-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5b135-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="5b135-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b135-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b135-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b135-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b135-106">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="5b135-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="5b135-107">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5b135-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5b135-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5b135-108">Methods</span></span>
|<span data-ttu-id="5b135-109">Método</span><span class="sxs-lookup"><span data-stu-id="5b135-109">Method</span></span>|<span data-ttu-id="5b135-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b135-110">Return Type</span></span>|<span data-ttu-id="5b135-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b135-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b135-112">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="5b135-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="5b135-113">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="5b135-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="5b135-114">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="5b135-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="5b135-115">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5b135-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="5b135-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5b135-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="5b135-117">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="5b135-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b135-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b135-118">Properties</span></span>
|<span data-ttu-id="5b135-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b135-119">Property</span></span>|<span data-ttu-id="5b135-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b135-120">Type</span></span>|<span data-ttu-id="5b135-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b135-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b135-122">displayName</span><span class="sxs-lookup"><span data-stu-id="5b135-122">displayName</span></span>|<span data-ttu-id="5b135-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b135-123">String</span></span>|<span data-ttu-id="5b135-124">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="5b135-124">Friendly name of the status report.</span></span> <span data-ttu-id="5b135-125">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5b135-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5b135-126">id</span><span class="sxs-lookup"><span data-stu-id="5b135-126">id</span></span>|<span data-ttu-id="5b135-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b135-127">String</span></span>|<span data-ttu-id="5b135-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b135-128">Key of the entity.</span></span> <span data-ttu-id="5b135-129">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5b135-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5b135-130">version</span><span class="sxs-lookup"><span data-stu-id="5b135-130">version</span></span>|<span data-ttu-id="5b135-131">String</span><span class="sxs-lookup"><span data-stu-id="5b135-131">String</span></span>|<span data-ttu-id="5b135-132">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5b135-132">Version of the entity.</span></span> <span data-ttu-id="5b135-133">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5b135-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="5b135-134">content</span><span class="sxs-lookup"><span data-stu-id="5b135-134">content</span></span>|[<span data-ttu-id="5b135-135">Json</span><span class="sxs-lookup"><span data-stu-id="5b135-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="5b135-136">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="5b135-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b135-137">Relações</span><span class="sxs-lookup"><span data-stu-id="5b135-137">Relationships</span></span>
<span data-ttu-id="5b135-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5b135-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b135-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b135-139">JSON Representation</span></span>
<span data-ttu-id="5b135-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b135-140">Here is a JSON representation of the resource.</span></span>
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




