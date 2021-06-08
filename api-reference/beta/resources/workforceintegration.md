---
title: Tipo de recurso workforceIntegration
description: Uma instância de integração de força de trabalho com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 12aa4a6ac8fd72f20a0019a95eeb20196b1ed3bf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787650"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="77790-103">Tipo de recurso workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="77790-103">workforceIntegration resource type</span></span>

<span data-ttu-id="77790-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77790-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77790-105">Uma instância de integração de força de trabalho com turnos.</span><span class="sxs-lookup"><span data-stu-id="77790-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="77790-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="77790-106">Methods</span></span>

| <span data-ttu-id="77790-107">Método</span><span class="sxs-lookup"><span data-stu-id="77790-107">Method</span></span>       | <span data-ttu-id="77790-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="77790-108">Return Type</span></span> | <span data-ttu-id="77790-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77790-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77790-110">List</span><span class="sxs-lookup"><span data-stu-id="77790-110">List</span></span>](../api/workforceintegration-list.md) | <span data-ttu-id="77790-111">[coleção workforceIntegration](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="77790-111">[workforceIntegration](workforceintegration.md) collection</span></span> | <span data-ttu-id="77790-112">Obter a lista de **objetos workforceIntegration** associados a essa agenda.</span><span class="sxs-lookup"><span data-stu-id="77790-112">Get the list of **workforceIntegration** objects associated with this schedule.</span></span>|
| [<span data-ttu-id="77790-113">Create</span><span class="sxs-lookup"><span data-stu-id="77790-113">Create</span></span>](../api/workforceintegration-post.md) | [<span data-ttu-id="77790-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="77790-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="77790-115">Crie um novo **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="77790-115">Create a new **workforceIntegration** object.</span></span>|
| [<span data-ttu-id="77790-116">Get</span><span class="sxs-lookup"><span data-stu-id="77790-116">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="77790-117">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="77790-117">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="77790-118">Leia as propriedades e as relações de um **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="77790-118">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="77790-119">Atualizar</span><span class="sxs-lookup"><span data-stu-id="77790-119">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="77790-120">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="77790-120">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="77790-121">Atualizar um **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="77790-121">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="77790-122">Delete</span><span class="sxs-lookup"><span data-stu-id="77790-122">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="77790-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="77790-123">None</span></span> | <span data-ttu-id="77790-124">Excluir um **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="77790-124">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77790-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77790-125">Properties</span></span>

| <span data-ttu-id="77790-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77790-126">Property</span></span>     | <span data-ttu-id="77790-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="77790-127">Type</span></span>        | <span data-ttu-id="77790-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="77790-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77790-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="77790-129">apiVersion</span></span>|<span data-ttu-id="77790-130">Int32</span><span class="sxs-lookup"><span data-stu-id="77790-130">Int32</span></span>|<span data-ttu-id="77790-131">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="77790-131">API version for the call back URL.</span></span> <span data-ttu-id="77790-132">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="77790-132">Start with 1.</span></span>|
|<span data-ttu-id="77790-133">displayName</span><span class="sxs-lookup"><span data-stu-id="77790-133">displayName</span></span>|<span data-ttu-id="77790-134">String</span><span class="sxs-lookup"><span data-stu-id="77790-134">String</span></span>|<span data-ttu-id="77790-135">Nome da integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="77790-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="77790-136">encryption</span><span class="sxs-lookup"><span data-stu-id="77790-136">encryption</span></span>|[<span data-ttu-id="77790-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="77790-137">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="77790-138">O recurso de criptografia de integração de força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="77790-138">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="77790-139">isActive</span><span class="sxs-lookup"><span data-stu-id="77790-139">isActive</span></span>|<span data-ttu-id="77790-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="77790-140">Boolean</span></span>|<span data-ttu-id="77790-141">Indica se essa integração de força de trabalho está ativa e disponível no momento.</span><span class="sxs-lookup"><span data-stu-id="77790-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="77790-142">suporta</span><span class="sxs-lookup"><span data-stu-id="77790-142">supports</span></span>|<span data-ttu-id="77790-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77790-143">string</span></span>| <span data-ttu-id="77790-144">As entidades Shifts suportadas para notificações de alteração síncrona.</span><span class="sxs-lookup"><span data-stu-id="77790-144">The Shifts entities supported for synchronous change notifications.</span></span> <span data-ttu-id="77790-145">Os turnos retornarão a url fornecida nas alterações do cliente nessas entidades adicionadas aqui.</span><span class="sxs-lookup"><span data-stu-id="77790-145">Shifts will make a call back to the url provided on client changes on those entities added here.</span></span> <span data-ttu-id="77790-146">Por padrão, nenhuma entidade tem suporte para notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="77790-146">By default, no entities are supported for change notifications.</span></span> <span data-ttu-id="77790-147">Os valores `none` possíveis `shift` são , , , , , , , , `swapRequest` , e `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="77790-147">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`, `offerShiftRequest`, `timeCard`, `timeOffReason`, `timeOff`, `timeOffRequest` and `unknownFutureValue`.</span></span> <span data-ttu-id="77790-148">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.</span><span class="sxs-lookup"><span data-stu-id="77790-148">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="77790-149">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="77790-149">supportedEntities</span></span>|<span data-ttu-id="77790-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77790-150">string</span></span>| <span data-ttu-id="77790-151">Essa propriedade substituirá **os suportes** em v1.0.</span><span class="sxs-lookup"><span data-stu-id="77790-151">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="77790-152">Recomendamos que você use essa propriedade em vez de **suporte**.</span><span class="sxs-lookup"><span data-stu-id="77790-152">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="77790-153">A **propriedade supports** ainda terá suporte na versão beta por enquanto.</span><span class="sxs-lookup"><span data-stu-id="77790-153">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="77790-154">Os valores `none` possíveis `shift` são , , , , , , , , `swapRequest` , e `openshift` `openShiftRequest` `userShiftPreferences` `offerShiftRequest` `timeCard` `timeOffReason` `timeOff` `timeOffRequest` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="77790-154">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`, `offerShiftRequest`, `timeCard`, `timeOffReason`, `timeOff`, `timeOffRequest` and `unknownFutureValue`.</span></span> <span data-ttu-id="77790-155">Se selecionar mais de um valor, todos os valores devem começar com a primeira letra em maiúscula.</span><span class="sxs-lookup"><span data-stu-id="77790-155">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="77790-156">url</span><span class="sxs-lookup"><span data-stu-id="77790-156">url</span></span>|<span data-ttu-id="77790-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77790-157">String</span></span>| <span data-ttu-id="77790-158">URL de Integração de Força de Trabalho para retornos de chamada do serviço Shifts.</span><span class="sxs-lookup"><span data-stu-id="77790-158">Workforce Integration URL for callbacks from the Shifts service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77790-159">Relações</span><span class="sxs-lookup"><span data-stu-id="77790-159">Relationships</span></span>

<span data-ttu-id="77790-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77790-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77790-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77790-161">JSON representation</span></span>

<span data-ttu-id="77790-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77790-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration"
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


