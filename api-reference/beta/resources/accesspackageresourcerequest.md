---
title: tipo de recurso accessPackageResourceRequest
description: Uma solicitação de recurso de pacote do Access é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74cc7815d4df22c1914f525ed0451b778c7777d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508517"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="ca810-103">tipo de recurso accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="ca810-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="ca810-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ca810-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca810-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de recurso de pacote do Access é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais dos pacotes de acesso do catálogo.</span><span class="sxs-lookup"><span data-stu-id="ca810-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="ca810-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca810-106">Methods</span></span>

| <span data-ttu-id="ca810-107">Método</span><span class="sxs-lookup"><span data-stu-id="ca810-107">Method</span></span>       | <span data-ttu-id="ca810-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ca810-108">Return Type</span></span> | <span data-ttu-id="ca810-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca810-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ca810-110">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="ca810-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="ca810-111">coleção [accessPackageResourceRequest](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ca810-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="ca810-112">Recupere uma lista de objetos **accessPackageResourceRequest** .</span><span class="sxs-lookup"><span data-stu-id="ca810-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="ca810-113">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="ca810-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="ca810-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="ca810-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="ca810-115">Criar um novo objeto **accessPackageResourceRequest** .</span><span class="sxs-lookup"><span data-stu-id="ca810-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca810-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca810-116">Properties</span></span>

| <span data-ttu-id="ca810-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca810-117">Property</span></span>     | <span data-ttu-id="ca810-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca810-118">Type</span></span>        | <span data-ttu-id="ca810-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca810-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca810-120">catalogID</span><span class="sxs-lookup"><span data-stu-id="ca810-120">catalogId</span></span>|<span data-ttu-id="ca810-121">String</span><span class="sxs-lookup"><span data-stu-id="ca810-121">String</span></span>|<span data-ttu-id="ca810-122">A ID exclusiva do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="ca810-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="ca810-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca810-123">expirationDateTime</span></span>|<span data-ttu-id="ca810-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca810-124">DateTimeOffset</span></span>|<span data-ttu-id="ca810-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca810-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca810-127">id</span><span class="sxs-lookup"><span data-stu-id="ca810-127">id</span></span>|<span data-ttu-id="ca810-128">String</span><span class="sxs-lookup"><span data-stu-id="ca810-128">String</span></span>| <span data-ttu-id="ca810-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca810-129">Read-only.</span></span>|
|<span data-ttu-id="ca810-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="ca810-130">isValidationOnly</span></span>|<span data-ttu-id="ca810-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca810-131">Boolean</span></span>|<span data-ttu-id="ca810-132">Se definido, não adiciona o recurso.</span><span class="sxs-lookup"><span data-stu-id="ca810-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="ca810-133">elabora</span><span class="sxs-lookup"><span data-stu-id="ca810-133">justification</span></span>|<span data-ttu-id="ca810-134">String</span><span class="sxs-lookup"><span data-stu-id="ca810-134">String</span></span>|<span data-ttu-id="ca810-135">A justificativa do solicitante para adicionar o recurso.</span><span class="sxs-lookup"><span data-stu-id="ca810-135">The requestor's justification for adding the resource.</span></span>|
|<span data-ttu-id="ca810-136">RequestState</span><span class="sxs-lookup"><span data-stu-id="ca810-136">requestState</span></span>|<span data-ttu-id="ca810-137">String</span><span class="sxs-lookup"><span data-stu-id="ca810-137">String</span></span>| <span data-ttu-id="ca810-138">O resultado de se o serviço foi capaz de adicionar o recurso ao catálogo.</span><span class="sxs-lookup"><span data-stu-id="ca810-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="ca810-139">O valor é `Delivered` se o recurso foi adicionado.</span><span class="sxs-lookup"><span data-stu-id="ca810-139">The value is `Delivered` if the resource was added.</span></span> <span data-ttu-id="ca810-140">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ca810-140">Read-Only.</span></span>|
|<span data-ttu-id="ca810-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="ca810-141">requestStatus</span></span>|<span data-ttu-id="ca810-142">String</span><span class="sxs-lookup"><span data-stu-id="ca810-142">String</span></span>|<span data-ttu-id="ca810-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca810-143">Read-only.</span></span>|
|<span data-ttu-id="ca810-144">RequestType</span><span class="sxs-lookup"><span data-stu-id="ca810-144">requestType</span></span>|<span data-ttu-id="ca810-145">String</span><span class="sxs-lookup"><span data-stu-id="ca810-145">String</span></span>|<span data-ttu-id="ca810-146">Use `AdminAdd` para adicionar um recurso se o chamador for um administrador ou proprietário de recurso.</span><span class="sxs-lookup"><span data-stu-id="ca810-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ca810-147">Relações</span><span class="sxs-lookup"><span data-stu-id="ca810-147">Relationships</span></span>

| <span data-ttu-id="ca810-148">Relação</span><span class="sxs-lookup"><span data-stu-id="ca810-148">Relationship</span></span> | <span data-ttu-id="ca810-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca810-149">Type</span></span>        | <span data-ttu-id="ca810-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca810-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca810-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="ca810-151">accessPackageResource</span></span>|[<span data-ttu-id="ca810-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="ca810-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="ca810-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca810-153">Nullable.</span></span>|
|<span data-ttu-id="ca810-154">solicitante</span><span class="sxs-lookup"><span data-stu-id="ca810-154">requestor</span></span>|[<span data-ttu-id="ca810-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ca810-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ca810-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ca810-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca810-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca810-158">JSON representation</span></span>

<span data-ttu-id="ca810-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca810-159">The following is a JSON representation of the resource.</span></span>

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
