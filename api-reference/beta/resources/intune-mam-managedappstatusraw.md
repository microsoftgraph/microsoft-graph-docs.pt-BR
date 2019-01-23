---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399259"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="22980-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="22980-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="22980-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="22980-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22980-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22980-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="22980-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22980-107">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="22980-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="22980-108">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22980-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="22980-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="22980-109">Methods</span></span>
|<span data-ttu-id="22980-110">Método</span><span class="sxs-lookup"><span data-stu-id="22980-110">Method</span></span>|<span data-ttu-id="22980-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22980-111">Return Type</span></span>|<span data-ttu-id="22980-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="22980-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22980-113">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="22980-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="22980-114">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="22980-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="22980-115">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="22980-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="22980-116">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="22980-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="22980-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="22980-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="22980-118">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="22980-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22980-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22980-119">Properties</span></span>
|<span data-ttu-id="22980-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22980-120">Property</span></span>|<span data-ttu-id="22980-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="22980-121">Type</span></span>|<span data-ttu-id="22980-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22980-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22980-123">displayName</span><span class="sxs-lookup"><span data-stu-id="22980-123">displayName</span></span>|<span data-ttu-id="22980-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22980-124">String</span></span>|<span data-ttu-id="22980-125">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="22980-125">Friendly name of the status report.</span></span> <span data-ttu-id="22980-126">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22980-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="22980-127">id</span><span class="sxs-lookup"><span data-stu-id="22980-127">id</span></span>|<span data-ttu-id="22980-128">String</span><span class="sxs-lookup"><span data-stu-id="22980-128">String</span></span>|<span data-ttu-id="22980-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22980-129">Key of the entity.</span></span> <span data-ttu-id="22980-130">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22980-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="22980-131">version</span><span class="sxs-lookup"><span data-stu-id="22980-131">version</span></span>|<span data-ttu-id="22980-132">String</span><span class="sxs-lookup"><span data-stu-id="22980-132">String</span></span>|<span data-ttu-id="22980-133">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="22980-133">Version of the entity.</span></span> <span data-ttu-id="22980-134">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22980-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="22980-135">content</span><span class="sxs-lookup"><span data-stu-id="22980-135">content</span></span>|[<span data-ttu-id="22980-136">Json</span><span class="sxs-lookup"><span data-stu-id="22980-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="22980-137">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="22980-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22980-138">Relações</span><span class="sxs-lookup"><span data-stu-id="22980-138">Relationships</span></span>
<span data-ttu-id="22980-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22980-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22980-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22980-140">JSON Representation</span></span>
<span data-ttu-id="22980-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22980-141">Here is a JSON representation of the resource.</span></span>
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




