---
title: tipo de recurso accessPackageResourceRequest
description: Uma solicitação de recurso de pacote do Access é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c109c2c28a9c4c9248adfbad4c94c9c50268f28f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871743"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="ee6be-103">tipo de recurso accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="ee6be-103">accessPackageResourceRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee6be-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de recurso de pacote do Access é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais dos pacotes de acesso do catálogo.</span><span class="sxs-lookup"><span data-stu-id="ee6be-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="ee6be-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee6be-105">Methods</span></span>

| <span data-ttu-id="ee6be-106">Método</span><span class="sxs-lookup"><span data-stu-id="ee6be-106">Method</span></span>       | <span data-ttu-id="ee6be-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee6be-107">Return Type</span></span> | <span data-ttu-id="ee6be-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee6be-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ee6be-109">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="ee6be-109">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="ee6be-110">coleção [accessPackageResourceRequest](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ee6be-110">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="ee6be-111">Recupere uma lista de objetos **accessPackageResourceRequest** .</span><span class="sxs-lookup"><span data-stu-id="ee6be-111">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="ee6be-112">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="ee6be-112">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="ee6be-113">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="ee6be-113">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="ee6be-114">Criar um novo objeto **accessPackageResourceRequest** .</span><span class="sxs-lookup"><span data-stu-id="ee6be-114">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ee6be-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee6be-115">Properties</span></span>

| <span data-ttu-id="ee6be-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee6be-116">Property</span></span>     | <span data-ttu-id="ee6be-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee6be-117">Type</span></span>        | <span data-ttu-id="ee6be-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee6be-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee6be-119">catalogID</span><span class="sxs-lookup"><span data-stu-id="ee6be-119">catalogId</span></span>|<span data-ttu-id="ee6be-120">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-120">String</span></span>|<span data-ttu-id="ee6be-121">A ID exclusiva do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="ee6be-121">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="ee6be-122">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ee6be-122">expirationDateTime</span></span>|<span data-ttu-id="ee6be-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee6be-123">DateTimeOffset</span></span>|<span data-ttu-id="ee6be-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ee6be-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ee6be-126">id</span><span class="sxs-lookup"><span data-stu-id="ee6be-126">id</span></span>|<span data-ttu-id="ee6be-127">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-127">String</span></span>| <span data-ttu-id="ee6be-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee6be-128">Read-only.</span></span>|
|<span data-ttu-id="ee6be-129">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="ee6be-129">isValidationOnly</span></span>|<span data-ttu-id="ee6be-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee6be-130">Boolean</span></span>|<span data-ttu-id="ee6be-131">Se definido, não adiciona o recurso.</span><span class="sxs-lookup"><span data-stu-id="ee6be-131">If set, does not add the resource.</span></span>|
|<span data-ttu-id="ee6be-132">elabora</span><span class="sxs-lookup"><span data-stu-id="ee6be-132">justification</span></span>|<span data-ttu-id="ee6be-133">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-133">String</span></span>|<span data-ttu-id="ee6be-134">A justificativa do solicitante para adicionar o recurso.</span><span class="sxs-lookup"><span data-stu-id="ee6be-134">The requestor's justification for adding the resource.</span></span>|
|<span data-ttu-id="ee6be-135">RequestState</span><span class="sxs-lookup"><span data-stu-id="ee6be-135">requestState</span></span>|<span data-ttu-id="ee6be-136">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-136">String</span></span>| <span data-ttu-id="ee6be-137">O resultado de se o serviço foi capaz de adicionar o recurso ao catálogo.</span><span class="sxs-lookup"><span data-stu-id="ee6be-137">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="ee6be-138">O valor é `Delivered` se o recurso foi adicionado.</span><span class="sxs-lookup"><span data-stu-id="ee6be-138">The value is `Delivered` if the resource was added.</span></span> <span data-ttu-id="ee6be-139">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ee6be-139">Read-Only.</span></span>|
|<span data-ttu-id="ee6be-140">requestStatus</span><span class="sxs-lookup"><span data-stu-id="ee6be-140">requestStatus</span></span>|<span data-ttu-id="ee6be-141">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-141">String</span></span>|<span data-ttu-id="ee6be-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee6be-142">Read-only.</span></span>|
|<span data-ttu-id="ee6be-143">RequestType</span><span class="sxs-lookup"><span data-stu-id="ee6be-143">requestType</span></span>|<span data-ttu-id="ee6be-144">String</span><span class="sxs-lookup"><span data-stu-id="ee6be-144">String</span></span>|<span data-ttu-id="ee6be-145">Use `AdminAdd` para adicionar um recurso se o chamador for um administrador ou proprietário de recurso.</span><span class="sxs-lookup"><span data-stu-id="ee6be-145">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ee6be-146">Relações</span><span class="sxs-lookup"><span data-stu-id="ee6be-146">Relationships</span></span>

| <span data-ttu-id="ee6be-147">Relação</span><span class="sxs-lookup"><span data-stu-id="ee6be-147">Relationship</span></span> | <span data-ttu-id="ee6be-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee6be-148">Type</span></span>        | <span data-ttu-id="ee6be-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee6be-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee6be-150">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="ee6be-150">accessPackageResource</span></span>|[<span data-ttu-id="ee6be-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="ee6be-151">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="ee6be-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee6be-152">Nullable.</span></span>|
|<span data-ttu-id="ee6be-153">solicitante</span><span class="sxs-lookup"><span data-stu-id="ee6be-153">requestor</span></span>|[<span data-ttu-id="ee6be-154">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ee6be-154">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ee6be-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee6be-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee6be-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee6be-157">JSON representation</span></span>

<span data-ttu-id="ee6be-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee6be-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
