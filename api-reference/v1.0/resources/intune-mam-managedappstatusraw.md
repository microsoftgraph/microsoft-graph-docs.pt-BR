---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d6b597f23cc10ba27b57cf5acbe5baf8bc9c328
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367011"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="f0866-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f0866-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="f0866-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0866-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0866-105">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="f0866-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="f0866-106">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f0866-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f0866-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0866-107">Methods</span></span>
|<span data-ttu-id="f0866-108">Método</span><span class="sxs-lookup"><span data-stu-id="f0866-108">Method</span></span>|<span data-ttu-id="f0866-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0866-109">Return Type</span></span>|<span data-ttu-id="f0866-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0866-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0866-111">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="f0866-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="f0866-112">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="f0866-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="f0866-113">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="f0866-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="f0866-114">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f0866-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="f0866-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f0866-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="f0866-116">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="f0866-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0866-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0866-117">Properties</span></span>
|<span data-ttu-id="f0866-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0866-118">Property</span></span>|<span data-ttu-id="f0866-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0866-119">Type</span></span>|<span data-ttu-id="f0866-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0866-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0866-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f0866-121">displayName</span></span>|<span data-ttu-id="f0866-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0866-122">String</span></span>|<span data-ttu-id="f0866-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="f0866-123">Friendly name of the status report.</span></span> <span data-ttu-id="f0866-124">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f0866-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f0866-125">id</span><span class="sxs-lookup"><span data-stu-id="f0866-125">id</span></span>|<span data-ttu-id="f0866-126">String</span><span class="sxs-lookup"><span data-stu-id="f0866-126">String</span></span>|<span data-ttu-id="f0866-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0866-127">Key of the entity.</span></span> <span data-ttu-id="f0866-128">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f0866-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f0866-129">version</span><span class="sxs-lookup"><span data-stu-id="f0866-129">version</span></span>|<span data-ttu-id="f0866-130">String</span><span class="sxs-lookup"><span data-stu-id="f0866-130">String</span></span>|<span data-ttu-id="f0866-131">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0866-131">Version of the entity.</span></span> <span data-ttu-id="f0866-132">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f0866-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f0866-133">content</span><span class="sxs-lookup"><span data-stu-id="f0866-133">content</span></span>|[<span data-ttu-id="f0866-134">Json</span><span class="sxs-lookup"><span data-stu-id="f0866-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="f0866-135">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="f0866-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0866-136">Relações</span><span class="sxs-lookup"><span data-stu-id="f0866-136">Relationships</span></span>
<span data-ttu-id="f0866-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0866-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0866-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0866-138">JSON Representation</span></span>
<span data-ttu-id="f0866-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0866-139">Here is a JSON representation of the resource.</span></span>
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




