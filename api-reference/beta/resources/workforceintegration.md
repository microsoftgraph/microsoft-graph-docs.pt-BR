---
title: tipo de recurso workforceIntegration
description: Uma instância de uma integração de força de funcionários com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 631f2cc52b9327d77edd6fc5ad48292cf044570f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866487"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="d6a1e-103">tipo de recurso workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="d6a1e-103">workforceIntegration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6a1e-104">Uma instância de uma integração de força de funcionários com turnos.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-104">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="d6a1e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6a1e-105">Methods</span></span>

| <span data-ttu-id="d6a1e-106">Método</span><span class="sxs-lookup"><span data-stu-id="d6a1e-106">Method</span></span>       | <span data-ttu-id="d6a1e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6a1e-107">Return Type</span></span> | <span data-ttu-id="d6a1e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6a1e-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d6a1e-109">Get</span><span class="sxs-lookup"><span data-stu-id="d6a1e-109">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="d6a1e-110">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="d6a1e-110">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="d6a1e-111">Leia as propriedades e os relacionamentos de um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="d6a1e-111">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="d6a1e-112">Update</span><span class="sxs-lookup"><span data-stu-id="d6a1e-112">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="d6a1e-113">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="d6a1e-113">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="d6a1e-114">Atualizar um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="d6a1e-114">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="d6a1e-115">Delete</span><span class="sxs-lookup"><span data-stu-id="d6a1e-115">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="d6a1e-116">None</span><span class="sxs-lookup"><span data-stu-id="d6a1e-116">None</span></span> | <span data-ttu-id="d6a1e-117">Excluir um objeto **workforceIntegration** .</span><span class="sxs-lookup"><span data-stu-id="d6a1e-117">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6a1e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6a1e-118">Properties</span></span>

| <span data-ttu-id="d6a1e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6a1e-119">Property</span></span>     | <span data-ttu-id="d6a1e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6a1e-120">Type</span></span>        | <span data-ttu-id="d6a1e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6a1e-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6a1e-122">apiVersion</span><span class="sxs-lookup"><span data-stu-id="d6a1e-122">apiVersion</span></span>|<span data-ttu-id="d6a1e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="d6a1e-123">Int32</span></span>|<span data-ttu-id="d6a1e-124">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-124">API version for the call back URL.</span></span> <span data-ttu-id="d6a1e-125">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-125">Start with 1.</span></span>|
|<span data-ttu-id="d6a1e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d6a1e-126">displayName</span></span>|<span data-ttu-id="d6a1e-127">String</span><span class="sxs-lookup"><span data-stu-id="d6a1e-127">String</span></span>|<span data-ttu-id="d6a1e-128">Nome da integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-128">Name of the workforce integration.</span></span>|
|<span data-ttu-id="d6a1e-129">encripta</span><span class="sxs-lookup"><span data-stu-id="d6a1e-129">encryption</span></span>|[<span data-ttu-id="d6a1e-130">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="d6a1e-130">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="d6a1e-131">O recurso de criptografia de integração da força de funcionários.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-131">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="d6a1e-132">isActive</span><span class="sxs-lookup"><span data-stu-id="d6a1e-132">isActive</span></span>|<span data-ttu-id="d6a1e-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6a1e-133">Boolean</span></span>|<span data-ttu-id="d6a1e-134">Indica se a integração da força de trabalho está ativa e disponível atualmente.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-134">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="d6a1e-135">compatível</span><span class="sxs-lookup"><span data-stu-id="d6a1e-135">supports</span></span>|<span data-ttu-id="d6a1e-136">string</span><span class="sxs-lookup"><span data-stu-id="d6a1e-136">string</span></span>| <span data-ttu-id="d6a1e-137">Os valores possíveis são `none`: `shift`, `swapRequest`, `openshift`, `openShiftRequest`,,`userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="d6a1e-137">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="d6a1e-138">url</span><span class="sxs-lookup"><span data-stu-id="d6a1e-138">url</span></span>|<span data-ttu-id="d6a1e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6a1e-139">String</span></span>| <span data-ttu-id="d6a1e-140">URL de integração de força de obra para retornos de chamada do serviço de turno.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-140">Workforce Integration URL for callbacks from the shift service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6a1e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d6a1e-141">Relationships</span></span>

<span data-ttu-id="d6a1e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6a1e-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6a1e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6a1e-143">JSON representation</span></span>

<span data-ttu-id="d6a1e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6a1e-144">The following is a JSON representation of the resource.</span></span>

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
