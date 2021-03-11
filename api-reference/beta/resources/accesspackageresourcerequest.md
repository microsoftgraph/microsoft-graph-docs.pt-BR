---
title: Tipo de recurso accessPackageResourceRequest
description: Uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea0d6ae14d93fbc691af4713cf40452a890d1891
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722185"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="1096b-103">Tipo de recurso accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="1096b-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="1096b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1096b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1096b-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de recurso do pacote de acesso é uma solicitação para adicionar um recurso a um catálogo para que as funções do recurso possam ser usadas em um ou mais pacotes de acesso do catálogo ou para remover um recurso de um catálogo que não seja mais necessário pelos pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="1096b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="1096b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1096b-106">Methods</span></span>

| <span data-ttu-id="1096b-107">Método</span><span class="sxs-lookup"><span data-stu-id="1096b-107">Method</span></span>       | <span data-ttu-id="1096b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1096b-108">Return Type</span></span> | <span data-ttu-id="1096b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1096b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1096b-110">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="1096b-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="1096b-111">[Coleção accessPackageResourceRequest](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="1096b-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="1096b-112">Recupere uma lista de **objetos accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="1096b-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="1096b-113">Criar accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="1096b-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="1096b-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1096b-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="1096b-115">Crie um novo **objeto accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="1096b-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1096b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1096b-116">Properties</span></span>

| <span data-ttu-id="1096b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1096b-117">Property</span></span>     | <span data-ttu-id="1096b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1096b-118">Type</span></span>        | <span data-ttu-id="1096b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1096b-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1096b-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="1096b-120">catalogId</span></span>|<span data-ttu-id="1096b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1096b-121">String</span></span>|<span data-ttu-id="1096b-122">A ID exclusiva do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="1096b-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="1096b-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1096b-123">expirationDateTime</span></span>|<span data-ttu-id="1096b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1096b-124">DateTimeOffset</span></span>|<span data-ttu-id="1096b-125">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1096b-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1096b-126">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1096b-126">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1096b-127">id</span><span class="sxs-lookup"><span data-stu-id="1096b-127">id</span></span>|<span data-ttu-id="1096b-128">String</span><span class="sxs-lookup"><span data-stu-id="1096b-128">String</span></span>| <span data-ttu-id="1096b-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1096b-129">Read-only.</span></span>|
|<span data-ttu-id="1096b-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="1096b-130">isValidationOnly</span></span>|<span data-ttu-id="1096b-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="1096b-131">Boolean</span></span>|<span data-ttu-id="1096b-132">Se definido, não adiciona o recurso.</span><span class="sxs-lookup"><span data-stu-id="1096b-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="1096b-133">justification</span><span class="sxs-lookup"><span data-stu-id="1096b-133">justification</span></span>|<span data-ttu-id="1096b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1096b-134">String</span></span>|<span data-ttu-id="1096b-135">A justificativa do solicitante para adicionar ou remover o recurso.</span><span class="sxs-lookup"><span data-stu-id="1096b-135">The requestor's justification for adding or removing the resource.</span></span>|
|<span data-ttu-id="1096b-136">requestState</span><span class="sxs-lookup"><span data-stu-id="1096b-136">requestState</span></span>|<span data-ttu-id="1096b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1096b-137">String</span></span>| <span data-ttu-id="1096b-138">O resultado se o serviço foi capaz de adicionar o recurso ao catálogo.</span><span class="sxs-lookup"><span data-stu-id="1096b-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="1096b-139">O valor é `Delivered` se o recurso foi adicionado ou removido.</span><span class="sxs-lookup"><span data-stu-id="1096b-139">The value is `Delivered` if the resource was added or removed.</span></span> <span data-ttu-id="1096b-140">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1096b-140">Read-Only.</span></span>|
|<span data-ttu-id="1096b-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="1096b-141">requestStatus</span></span>|<span data-ttu-id="1096b-142">String</span><span class="sxs-lookup"><span data-stu-id="1096b-142">String</span></span>|<span data-ttu-id="1096b-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1096b-143">Read-only.</span></span>|
|<span data-ttu-id="1096b-144">requestType</span><span class="sxs-lookup"><span data-stu-id="1096b-144">requestType</span></span>|<span data-ttu-id="1096b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1096b-145">String</span></span>|<span data-ttu-id="1096b-146">Use `AdminAdd` para adicionar um recurso, se o chamador for um administrador ou proprietário de recursos ou para remover um `AdminRemove` recurso.</span><span class="sxs-lookup"><span data-stu-id="1096b-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner, or `AdminRemove` to remove a resource.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1096b-147">Relações</span><span class="sxs-lookup"><span data-stu-id="1096b-147">Relationships</span></span>

| <span data-ttu-id="1096b-148">Relação</span><span class="sxs-lookup"><span data-stu-id="1096b-148">Relationship</span></span> | <span data-ttu-id="1096b-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="1096b-149">Type</span></span>        | <span data-ttu-id="1096b-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="1096b-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1096b-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1096b-151">accessPackageResource</span></span>|[<span data-ttu-id="1096b-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1096b-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="1096b-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1096b-153">Nullable.</span></span>|
|<span data-ttu-id="1096b-154">requestor</span><span class="sxs-lookup"><span data-stu-id="1096b-154">requestor</span></span>|[<span data-ttu-id="1096b-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="1096b-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="1096b-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1096b-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1096b-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1096b-158">JSON representation</span></span>

<span data-ttu-id="1096b-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1096b-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
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


