---
title: 'Grupo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de grupo especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45842a31bb4e7a7b2ec3e5405aa17c4cf6a5a53d
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041800"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="dbc5b-103">Grupo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="dbc5b-103">group: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc5b-104">Verifique se há associação em uma lista de grupos ou unidades administrativas para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-104">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="dbc5b-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbc5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbc5b-106">Permissions</span></span>

<span data-ttu-id="dbc5b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbc5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbc5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbc5b-109">Permission type</span></span>                        | <span data-ttu-id="dbc5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbc5b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dbc5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbc5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbc5b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="dbc5b-113">E</span><span class="sxs-lookup"><span data-stu-id="dbc5b-113">And:</span></span><br><ul><li><span data-ttu-id="dbc5b-114">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="dbc5b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="dbc5b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbc5b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbc5b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-117">Not supported.</span></span> |
| <span data-ttu-id="dbc5b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbc5b-118">Application</span></span>                            | <span data-ttu-id="dbc5b-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="dbc5b-120">E</span><span class="sxs-lookup"><span data-stu-id="dbc5b-120">And:</span></span><br><ul><li><span data-ttu-id="dbc5b-121">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="dbc5b-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbc5b-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbc5b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc5b-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="dbc5b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc5b-124">Request headers</span></span>

| <span data-ttu-id="dbc5b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="dbc5b-125">Name</span></span>          | <span data-ttu-id="dbc5b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbc5b-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dbc5b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbc5b-127">Authorization</span></span> | <span data-ttu-id="dbc5b-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dbc5b-128">Bearer {token}</span></span> |
| <span data-ttu-id="dbc5b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbc5b-129">Content-Type</span></span>  | <span data-ttu-id="dbc5b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="dbc5b-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbc5b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc5b-131">Request body</span></span>

<span data-ttu-id="dbc5b-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbc5b-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dbc5b-133">Parameter</span></span>    | <span data-ttu-id="dbc5b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbc5b-134">Type</span></span>        | <span data-ttu-id="dbc5b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbc5b-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbc5b-136">ids</span><span class="sxs-lookup"><span data-stu-id="dbc5b-136">ids</span></span>|<span data-ttu-id="dbc5b-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbc5b-137">String collection</span></span>| <span data-ttu-id="dbc5b-138">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-138">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="dbc5b-139">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-139">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="dbc5b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc5b-140">Response</span></span>

<span data-ttu-id="dbc5b-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbc5b-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dbc5b-142">Examples</span></span>

<span data-ttu-id="dbc5b-143">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-143">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dbc5b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc5b-144">Request</span></span>

<span data-ttu-id="dbc5b-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-145">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dbc5b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc5b-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbc5b-147">C#</span><span class="sxs-lookup"><span data-stu-id="dbc5b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbc5b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbc5b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbc5b-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dbc5b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dbc5b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc5b-150">Response</span></span>

<span data-ttu-id="dbc5b-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-151">The following is an example of the response.</span></span> 

> <span data-ttu-id="dbc5b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbc5b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
