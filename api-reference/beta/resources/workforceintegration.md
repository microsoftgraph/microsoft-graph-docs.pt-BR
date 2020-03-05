---
title: tipo de recurso workforceIntegration
description: Uma instância de uma integração de força de funcionários com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519082"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="52b83-103">tipo de recurso workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="52b83-103">workforceIntegration resource type</span></span>

<span data-ttu-id="52b83-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52b83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b83-105">Uma instância de uma integração de força de funcionários com turnos.</span><span class="sxs-lookup"><span data-stu-id="52b83-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="52b83-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52b83-106">Methods</span></span>

| <span data-ttu-id="52b83-107">Método</span><span class="sxs-lookup"><span data-stu-id="52b83-107">Method</span></span>       | <span data-ttu-id="52b83-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52b83-108">Return Type</span></span> | <span data-ttu-id="52b83-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b83-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52b83-110">Get</span><span class="sxs-lookup"><span data-stu-id="52b83-110">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="52b83-111">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="52b83-111">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="52b83-112">Leia as propriedades e os relacionamentos de um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="52b83-112">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="52b83-113">Update</span><span class="sxs-lookup"><span data-stu-id="52b83-113">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="52b83-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="52b83-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="52b83-115">Atualizar um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="52b83-115">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="52b83-116">Delete</span><span class="sxs-lookup"><span data-stu-id="52b83-116">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="52b83-117">None</span><span class="sxs-lookup"><span data-stu-id="52b83-117">None</span></span> | <span data-ttu-id="52b83-118">Excluir um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="52b83-118">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52b83-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52b83-119">Properties</span></span>

| <span data-ttu-id="52b83-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52b83-120">Property</span></span>     | <span data-ttu-id="52b83-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="52b83-121">Type</span></span>        | <span data-ttu-id="52b83-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b83-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52b83-123">apiVersion</span><span class="sxs-lookup"><span data-stu-id="52b83-123">apiVersion</span></span>|<span data-ttu-id="52b83-124">Int32</span><span class="sxs-lookup"><span data-stu-id="52b83-124">Int32</span></span>|<span data-ttu-id="52b83-125">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="52b83-125">API version for the call back URL.</span></span> <span data-ttu-id="52b83-126">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="52b83-126">Start with 1.</span></span>|
|<span data-ttu-id="52b83-127">displayName</span><span class="sxs-lookup"><span data-stu-id="52b83-127">displayName</span></span>|<span data-ttu-id="52b83-128">String</span><span class="sxs-lookup"><span data-stu-id="52b83-128">String</span></span>|<span data-ttu-id="52b83-129">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="52b83-129">Name of the workforce integration.</span></span>|
|<span data-ttu-id="52b83-130">encripta</span><span class="sxs-lookup"><span data-stu-id="52b83-130">encryption</span></span>|[<span data-ttu-id="52b83-131">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="52b83-131">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="52b83-132">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="52b83-132">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="52b83-133">isActive</span><span class="sxs-lookup"><span data-stu-id="52b83-133">isActive</span></span>|<span data-ttu-id="52b83-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="52b83-134">Boolean</span></span>|<span data-ttu-id="52b83-135">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="52b83-135">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="52b83-136">compatível</span><span class="sxs-lookup"><span data-stu-id="52b83-136">supports</span></span>|<span data-ttu-id="52b83-137">string</span><span class="sxs-lookup"><span data-stu-id="52b83-137">string</span></span>| <span data-ttu-id="52b83-138">Os valores possíveis são `none`: `shift`, `swapRequest`, `openshift`, `openShiftRequest`,,`userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="52b83-138">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="52b83-139">url</span><span class="sxs-lookup"><span data-stu-id="52b83-139">url</span></span>|<span data-ttu-id="52b83-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52b83-140">String</span></span>| <span data-ttu-id="52b83-141">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="52b83-141">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52b83-142">Relações</span><span class="sxs-lookup"><span data-stu-id="52b83-142">Relationships</span></span>

<span data-ttu-id="52b83-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52b83-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52b83-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52b83-144">JSON representation</span></span>

<span data-ttu-id="52b83-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52b83-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supports": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
