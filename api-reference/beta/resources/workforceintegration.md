---
title: Tipo de recurso workforceIntegration
description: Uma instância de uma integração da força de trabalho com turnos.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b9e8678a009dab1f6e6cceae8b9ce98d1849cbd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158307"
---
# <a name="workforceintegration-resource-type"></a><span data-ttu-id="61222-103">Tipo de recurso workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61222-103">workforceIntegration resource type</span></span>

<span data-ttu-id="61222-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61222-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61222-105">Uma instância de uma integração da força de trabalho com turnos.</span><span class="sxs-lookup"><span data-stu-id="61222-105">An instance of a workforce integration with shifts.</span></span>

## <a name="methods"></a><span data-ttu-id="61222-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="61222-106">Methods</span></span>

| <span data-ttu-id="61222-107">Método</span><span class="sxs-lookup"><span data-stu-id="61222-107">Method</span></span>       | <span data-ttu-id="61222-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61222-108">Return Type</span></span> | <span data-ttu-id="61222-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="61222-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="61222-110">List</span><span class="sxs-lookup"><span data-stu-id="61222-110">List</span></span>](../api/workforceintegration-list.md) | <span data-ttu-id="61222-111">[coleção workforceIntegration](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="61222-111">[workforceIntegration](workforceintegration.md) collection</span></span> | <span data-ttu-id="61222-112">Obter a lista de **objetos workforceIntegration** associados a este cronograma.</span><span class="sxs-lookup"><span data-stu-id="61222-112">Get the list of **workforceIntegration** objects associated with this schedule.</span></span>|
| [<span data-ttu-id="61222-113">Criar</span><span class="sxs-lookup"><span data-stu-id="61222-113">Create</span></span>](../api/workforceintegration-post.md) | [<span data-ttu-id="61222-114">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61222-114">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="61222-115">Crie um novo **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="61222-115">Create a new **workforceIntegration** object.</span></span>|
| [<span data-ttu-id="61222-116">Get</span><span class="sxs-lookup"><span data-stu-id="61222-116">Get</span></span>](../api/workforceintegration-get.md) | [<span data-ttu-id="61222-117">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61222-117">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="61222-118">Leia as propriedades e os relacionamentos de um **objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="61222-118">Read the properties and relationships of a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="61222-119">Update</span><span class="sxs-lookup"><span data-stu-id="61222-119">Update</span></span>](../api/workforceintegration-update.md) | [<span data-ttu-id="61222-120">workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="61222-120">workforceIntegration</span></span>](workforceintegration.md) | <span data-ttu-id="61222-121">Atualize **um objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="61222-121">Update a **workforceIntegration** object.</span></span> |
| [<span data-ttu-id="61222-122">Delete</span><span class="sxs-lookup"><span data-stu-id="61222-122">Delete</span></span>](../api/workforceintegration-delete.md) | <span data-ttu-id="61222-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="61222-123">None</span></span> | <span data-ttu-id="61222-124">Exclua **um objeto workforceIntegration.**</span><span class="sxs-lookup"><span data-stu-id="61222-124">Delete a **workforceIntegration** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="61222-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61222-125">Properties</span></span>

| <span data-ttu-id="61222-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61222-126">Property</span></span>     | <span data-ttu-id="61222-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="61222-127">Type</span></span>        | <span data-ttu-id="61222-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="61222-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61222-129">apiVersion</span><span class="sxs-lookup"><span data-stu-id="61222-129">apiVersion</span></span>|<span data-ttu-id="61222-130">Int32</span><span class="sxs-lookup"><span data-stu-id="61222-130">Int32</span></span>|<span data-ttu-id="61222-131">Versão da API para a URL de retorno de chamada.</span><span class="sxs-lookup"><span data-stu-id="61222-131">API version for the call back URL.</span></span> <span data-ttu-id="61222-132">Comece com 1.</span><span class="sxs-lookup"><span data-stu-id="61222-132">Start with 1.</span></span>|
|<span data-ttu-id="61222-133">displayName</span><span class="sxs-lookup"><span data-stu-id="61222-133">displayName</span></span>|<span data-ttu-id="61222-134">String</span><span class="sxs-lookup"><span data-stu-id="61222-134">String</span></span>|<span data-ttu-id="61222-135">Nome da integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="61222-135">Name of the workforce integration.</span></span>|
|<span data-ttu-id="61222-136">criptografia</span><span class="sxs-lookup"><span data-stu-id="61222-136">encryption</span></span>|[<span data-ttu-id="61222-137">workforceIntegrationEncryption</span><span class="sxs-lookup"><span data-stu-id="61222-137">workforceIntegrationEncryption</span></span>](workforceintegrationencryption.md)|<span data-ttu-id="61222-138">O recurso de criptografia de integração da força de trabalho.</span><span class="sxs-lookup"><span data-stu-id="61222-138">The workforce integration encryption resource.</span></span>|
|<span data-ttu-id="61222-139">isActive</span><span class="sxs-lookup"><span data-stu-id="61222-139">isActive</span></span>|<span data-ttu-id="61222-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="61222-140">Boolean</span></span>|<span data-ttu-id="61222-141">Indica se essa integração de força de trabalho está ativa e disponível no momento.</span><span class="sxs-lookup"><span data-stu-id="61222-141">Indicates whether this workforce integration is currently active and available.</span></span>|
|<span data-ttu-id="61222-142">oferece suporte</span><span class="sxs-lookup"><span data-stu-id="61222-142">supports</span></span>|<span data-ttu-id="61222-143">string</span><span class="sxs-lookup"><span data-stu-id="61222-143">string</span></span>| <span data-ttu-id="61222-144">As entidades Shifts são suportadas para notificações de alteração síncrona.</span><span class="sxs-lookup"><span data-stu-id="61222-144">The Shifts entities supported for synchronous change notifications.</span></span> <span data-ttu-id="61222-145">Os turnos fazem uma chamada de volta para a URL fornecida nas alterações do cliente nessas entidades adicionadas aqui.</span><span class="sxs-lookup"><span data-stu-id="61222-145">Shifts will make a call back to the url provided on client changes on those entities added here.</span></span> <span data-ttu-id="61222-146">Por padrão, nenhuma entidade tem suporte para notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="61222-146">By default, no entities are supported for change notifications.</span></span> <span data-ttu-id="61222-147">Os valores possíveis `none` são: `shift` , , , `swapRequest` `openshift` , `openShiftRequest``userShiftPreferences`</span><span class="sxs-lookup"><span data-stu-id="61222-147">Possible values are: `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`</span></span>|
|<span data-ttu-id="61222-148">supportedEntities</span><span class="sxs-lookup"><span data-stu-id="61222-148">supportedEntities</span></span>|<span data-ttu-id="61222-149">string</span><span class="sxs-lookup"><span data-stu-id="61222-149">string</span></span>| <span data-ttu-id="61222-150">Essa propriedade substituirá **os suportes** na v1.0.</span><span class="sxs-lookup"><span data-stu-id="61222-150">This property will replace **supports** in v1.0.</span></span> <span data-ttu-id="61222-151">Recomendamos que você use essa propriedade em vez de **suporte.**</span><span class="sxs-lookup"><span data-stu-id="61222-151">We recommend that you use this property instead of **supports**.</span></span> <span data-ttu-id="61222-152">A **propriedade** supports ainda terá suporte na versão beta por enquanto.</span><span class="sxs-lookup"><span data-stu-id="61222-152">The **supports** property will still be supported in beta for the time being.</span></span> <span data-ttu-id="61222-153">Os valores possíveis `none` são , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` .</span><span class="sxs-lookup"><span data-stu-id="61222-153">Possible values are `none`, `shift`, `swapRequest`, `openshift`, `openShiftRequest`, `userShiftPreferences`.</span></span> <span data-ttu-id="61222-154">Se você selecionar mais de um valor, todos os valores deverão começar com a primeira letra em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="61222-154">If selecting more than one value, all values must start with the first letter in uppercase.</span></span>|
|<span data-ttu-id="61222-155">url</span><span class="sxs-lookup"><span data-stu-id="61222-155">url</span></span>|<span data-ttu-id="61222-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61222-156">String</span></span>| <span data-ttu-id="61222-157">URL de integração da força de trabalho para retornos de chamada do serviço Shifts.</span><span class="sxs-lookup"><span data-stu-id="61222-157">Workforce Integration URL for callbacks from the Shifts service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61222-158">Relações</span><span class="sxs-lookup"><span data-stu-id="61222-158">Relationships</span></span>

<span data-ttu-id="61222-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61222-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61222-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61222-160">JSON representation</span></span>

<span data-ttu-id="61222-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61222-161">The following is a JSON representation of the resource.</span></span>

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


