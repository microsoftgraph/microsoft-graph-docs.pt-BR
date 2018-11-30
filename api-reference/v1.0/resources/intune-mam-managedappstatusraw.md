---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
ms.openlocfilehash: 9576123e39be2ae37052926342fb634c21086371
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006522"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="21b4d-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21b4d-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="21b4d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21b4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21b4d-105">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="21b4d-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="21b4d-106">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="21b4d-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="21b4d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="21b4d-107">Methods</span></span>
|<span data-ttu-id="21b4d-108">Método</span><span class="sxs-lookup"><span data-stu-id="21b4d-108">Method</span></span>|<span data-ttu-id="21b4d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21b4d-109">Return Type</span></span>|<span data-ttu-id="21b4d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b4d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21b4d-111">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="21b4d-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="21b4d-112">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="21b4d-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="21b4d-113">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="21b4d-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="21b4d-114">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21b4d-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="21b4d-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="21b4d-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="21b4d-116">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="21b4d-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21b4d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21b4d-117">Properties</span></span>
|<span data-ttu-id="21b4d-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21b4d-118">Property</span></span>|<span data-ttu-id="21b4d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b4d-119">Type</span></span>|<span data-ttu-id="21b4d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b4d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21b4d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="21b4d-121">displayName</span></span>|<span data-ttu-id="21b4d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21b4d-122">String</span></span>|<span data-ttu-id="21b4d-123">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="21b4d-123">Friendly name of the status report.</span></span> <span data-ttu-id="21b4d-124">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="21b4d-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21b4d-125">id</span><span class="sxs-lookup"><span data-stu-id="21b4d-125">id</span></span>|<span data-ttu-id="21b4d-126">String</span><span class="sxs-lookup"><span data-stu-id="21b4d-126">String</span></span>|<span data-ttu-id="21b4d-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21b4d-127">Key of the entity.</span></span> <span data-ttu-id="21b4d-128">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="21b4d-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21b4d-129">version</span><span class="sxs-lookup"><span data-stu-id="21b4d-129">version</span></span>|<span data-ttu-id="21b4d-130">String</span><span class="sxs-lookup"><span data-stu-id="21b4d-130">String</span></span>|<span data-ttu-id="21b4d-131">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="21b4d-131">Version of the entity.</span></span> <span data-ttu-id="21b4d-132">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="21b4d-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="21b4d-133">content</span><span class="sxs-lookup"><span data-stu-id="21b4d-133">content</span></span>|[<span data-ttu-id="21b4d-134">Json</span><span class="sxs-lookup"><span data-stu-id="21b4d-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="21b4d-135">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="21b4d-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21b4d-136">Relações</span><span class="sxs-lookup"><span data-stu-id="21b4d-136">Relationships</span></span>
<span data-ttu-id="21b4d-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21b4d-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21b4d-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21b4d-138">JSON Representation</span></span>
<span data-ttu-id="21b4d-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21b4d-139">Here is a JSON representation of the resource.</span></span>
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



