---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c89b36f7b9587a99d280de789dcaa753442591e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465234"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="6257c-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="6257c-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="6257c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6257c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6257c-105">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="6257c-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="6257c-106">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6257c-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6257c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6257c-107">Methods</span></span>
|<span data-ttu-id="6257c-108">Método</span><span class="sxs-lookup"><span data-stu-id="6257c-108">Method</span></span>|<span data-ttu-id="6257c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6257c-109">Return Type</span></span>|<span data-ttu-id="6257c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6257c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6257c-111">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="6257c-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="6257c-112">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="6257c-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="6257c-113">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="6257c-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="6257c-114">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="6257c-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="6257c-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="6257c-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="6257c-116">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="6257c-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6257c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6257c-117">Properties</span></span>
|<span data-ttu-id="6257c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6257c-118">Property</span></span>|<span data-ttu-id="6257c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6257c-119">Type</span></span>|<span data-ttu-id="6257c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6257c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6257c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6257c-121">displayName</span></span>|<span data-ttu-id="6257c-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6257c-122">String</span></span>|<span data-ttu-id="6257c-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="6257c-123">Friendly name of the status report.</span></span> <span data-ttu-id="6257c-124">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6257c-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="6257c-125">id</span><span class="sxs-lookup"><span data-stu-id="6257c-125">id</span></span>|<span data-ttu-id="6257c-126">String</span><span class="sxs-lookup"><span data-stu-id="6257c-126">String</span></span>|<span data-ttu-id="6257c-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6257c-127">Key of the entity.</span></span> <span data-ttu-id="6257c-128">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6257c-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="6257c-129">version</span><span class="sxs-lookup"><span data-stu-id="6257c-129">version</span></span>|<span data-ttu-id="6257c-130">String</span><span class="sxs-lookup"><span data-stu-id="6257c-130">String</span></span>|<span data-ttu-id="6257c-131">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="6257c-131">Version of the entity.</span></span> <span data-ttu-id="6257c-132">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6257c-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="6257c-133">content</span><span class="sxs-lookup"><span data-stu-id="6257c-133">content</span></span>|[<span data-ttu-id="6257c-134">Json</span><span class="sxs-lookup"><span data-stu-id="6257c-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="6257c-135">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="6257c-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6257c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="6257c-136">Relationships</span></span>
<span data-ttu-id="6257c-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6257c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6257c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6257c-138">JSON Representation</span></span>
<span data-ttu-id="6257c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6257c-139">Here is a JSON representation of the resource.</span></span>
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



