---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 975f43d064718b8457b40be707a54a0ea0eb69f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884011"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="ea51f-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="ea51f-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="ea51f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea51f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea51f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea51f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea51f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea51f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea51f-107">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="ea51f-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="ea51f-108">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea51f-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ea51f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea51f-109">Methods</span></span>
|<span data-ttu-id="ea51f-110">Método</span><span class="sxs-lookup"><span data-stu-id="ea51f-110">Method</span></span>|<span data-ttu-id="ea51f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea51f-111">Return Type</span></span>|<span data-ttu-id="ea51f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea51f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea51f-113">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="ea51f-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="ea51f-114">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="ea51f-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="ea51f-115">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="ea51f-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="ea51f-116">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="ea51f-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="ea51f-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="ea51f-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="ea51f-118">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="ea51f-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea51f-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea51f-119">Properties</span></span>
|<span data-ttu-id="ea51f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea51f-120">Property</span></span>|<span data-ttu-id="ea51f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea51f-121">Type</span></span>|<span data-ttu-id="ea51f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea51f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea51f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="ea51f-123">displayName</span></span>|<span data-ttu-id="ea51f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea51f-124">String</span></span>|<span data-ttu-id="ea51f-125">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="ea51f-125">Friendly name of the status report.</span></span> <span data-ttu-id="ea51f-126">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea51f-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="ea51f-127">id</span><span class="sxs-lookup"><span data-stu-id="ea51f-127">id</span></span>|<span data-ttu-id="ea51f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea51f-128">String</span></span>|<span data-ttu-id="ea51f-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea51f-129">Key of the entity.</span></span> <span data-ttu-id="ea51f-130">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea51f-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="ea51f-131">version</span><span class="sxs-lookup"><span data-stu-id="ea51f-131">version</span></span>|<span data-ttu-id="ea51f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea51f-132">String</span></span>|<span data-ttu-id="ea51f-133">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea51f-133">Version of the entity.</span></span> <span data-ttu-id="ea51f-134">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea51f-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="ea51f-135">content</span><span class="sxs-lookup"><span data-stu-id="ea51f-135">content</span></span>|[<span data-ttu-id="ea51f-136">Json</span><span class="sxs-lookup"><span data-stu-id="ea51f-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="ea51f-137">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="ea51f-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea51f-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ea51f-138">Relationships</span></span>
<span data-ttu-id="ea51f-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea51f-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea51f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea51f-140">JSON Representation</span></span>
<span data-ttu-id="ea51f-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea51f-141">Here is a JSON representation of the resource.</span></span>
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





