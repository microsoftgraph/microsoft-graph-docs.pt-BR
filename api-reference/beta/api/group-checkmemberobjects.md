---
title: 'Grupo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de grupo especificado.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 38c362c8ef06ae230b1a4dfbf6a5d5436abf016d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123906"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="01d79-103">Grupo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="01d79-103">group: checkMemberObjects</span></span>

<span data-ttu-id="01d79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01d79-105">Verifique se há associação em uma lista de grupos ou unidades administrativas para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="01d79-105">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="01d79-106">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="01d79-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="01d79-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01d79-107">Permissions</span></span>

<span data-ttu-id="01d79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01d79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01d79-110">Permission type</span></span>                        | <span data-ttu-id="01d79-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01d79-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01d79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01d79-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01d79-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d79-113">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="01d79-114">E</span><span class="sxs-lookup"><span data-stu-id="01d79-114">And:</span></span><br><ul><li><span data-ttu-id="01d79-115">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="01d79-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="01d79-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01d79-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="01d79-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01d79-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01d79-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01d79-118">Not supported.</span></span> |
| <span data-ttu-id="01d79-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01d79-119">Application</span></span>                            | <span data-ttu-id="01d79-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d79-120">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="01d79-121">E</span><span class="sxs-lookup"><span data-stu-id="01d79-121">And:</span></span><br><ul><li><span data-ttu-id="01d79-122">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="01d79-122">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="01d79-123">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d79-123">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01d79-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01d79-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="01d79-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01d79-125">Request headers</span></span>

| <span data-ttu-id="01d79-126">Nome</span><span class="sxs-lookup"><span data-stu-id="01d79-126">Name</span></span>          | <span data-ttu-id="01d79-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d79-127">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="01d79-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="01d79-128">Authorization</span></span> | <span data-ttu-id="01d79-129">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="01d79-129">Bearer {token}</span></span> |
| <span data-ttu-id="01d79-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01d79-130">Content-Type</span></span>  | <span data-ttu-id="01d79-131">application/json</span><span class="sxs-lookup"><span data-stu-id="01d79-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01d79-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01d79-132">Request body</span></span>

<span data-ttu-id="01d79-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01d79-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01d79-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01d79-134">Parameter</span></span>    | <span data-ttu-id="01d79-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="01d79-135">Type</span></span>        | <span data-ttu-id="01d79-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d79-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01d79-137">ids</span><span class="sxs-lookup"><span data-stu-id="01d79-137">ids</span></span>|<span data-ttu-id="01d79-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="01d79-138">String collection</span></span>| <span data-ttu-id="01d79-139">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="01d79-139">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="01d79-140">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="01d79-140">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="01d79-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d79-141">Response</span></span>

<span data-ttu-id="01d79-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01d79-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01d79-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="01d79-143">Examples</span></span>

<span data-ttu-id="01d79-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="01d79-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="01d79-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01d79-145">Request</span></span>

<span data-ttu-id="01d79-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01d79-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01d79-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="01d79-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="01d79-148">C#</span><span class="sxs-lookup"><span data-stu-id="01d79-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01d79-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01d79-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01d79-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01d79-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01d79-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d79-151">Response</span></span>

<span data-ttu-id="01d79-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01d79-152">The following is an example of the response.</span></span> 

> <span data-ttu-id="01d79-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01d79-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
