---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
ms.openlocfilehash: 9b7c957451e3fc92ad79ef10433e26bf39fd1c48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331924"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="8e02e-103">tipo de recurso managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="8e02e-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="8e02e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e02e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e02e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e02e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e02e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8e02e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e02e-107">Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.</span><span class="sxs-lookup"><span data-stu-id="8e02e-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="8e02e-108">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8e02e-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8e02e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e02e-109">Methods</span></span>
|<span data-ttu-id="8e02e-110">Método</span><span class="sxs-lookup"><span data-stu-id="8e02e-110">Method</span></span>|<span data-ttu-id="8e02e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e02e-111">Return Type</span></span>|<span data-ttu-id="8e02e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e02e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e02e-113">Listar managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="8e02e-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="8e02e-114">Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)</span><span class="sxs-lookup"><span data-stu-id="8e02e-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="8e02e-115">Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="8e02e-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="8e02e-116">Obter managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="8e02e-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="8e02e-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="8e02e-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="8e02e-118">Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="8e02e-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e02e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e02e-119">Properties</span></span>
|<span data-ttu-id="8e02e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e02e-120">Property</span></span>|<span data-ttu-id="8e02e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e02e-121">Type</span></span>|<span data-ttu-id="8e02e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e02e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e02e-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8e02e-123">displayName</span></span>|<span data-ttu-id="8e02e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e02e-124">String</span></span>|<span data-ttu-id="8e02e-125">Nome amigável do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="8e02e-125">Friendly name of the status report.</span></span> <span data-ttu-id="8e02e-126">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8e02e-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8e02e-127">id</span><span class="sxs-lookup"><span data-stu-id="8e02e-127">id</span></span>|<span data-ttu-id="8e02e-128">String</span><span class="sxs-lookup"><span data-stu-id="8e02e-128">String</span></span>|<span data-ttu-id="8e02e-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e02e-129">Key of the entity.</span></span> <span data-ttu-id="8e02e-130">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8e02e-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8e02e-131">version</span><span class="sxs-lookup"><span data-stu-id="8e02e-131">version</span></span>|<span data-ttu-id="8e02e-132">String</span><span class="sxs-lookup"><span data-stu-id="8e02e-132">String</span></span>|<span data-ttu-id="8e02e-133">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e02e-133">Version of the entity.</span></span> <span data-ttu-id="8e02e-134">Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8e02e-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8e02e-135">content</span><span class="sxs-lookup"><span data-stu-id="8e02e-135">content</span></span>|[<span data-ttu-id="8e02e-136">Json</span><span class="sxs-lookup"><span data-stu-id="8e02e-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="8e02e-137">Conteúdo do relatório de status.</span><span class="sxs-lookup"><span data-stu-id="8e02e-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e02e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="8e02e-138">Relationships</span></span>
<span data-ttu-id="8e02e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e02e-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e02e-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e02e-140">JSON Representation</span></span>
<span data-ttu-id="8e02e-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e02e-141">Here is a JSON representation of the resource.</span></span>
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





