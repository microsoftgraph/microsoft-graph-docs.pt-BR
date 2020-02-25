---
title: 'usuário: checkMemberObjects'
description: Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 42e6ea9e258549448d77511756b892f3996e9379
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268368"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="20523-103">usuário: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="20523-103">user: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20523-104">Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="20523-104">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="20523-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="20523-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="20523-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20523-106">Permissions</span></span>

<span data-ttu-id="20523-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20523-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20523-109">Permission type</span></span>                        | <span data-ttu-id="20523-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20523-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20523-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20523-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20523-112">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-112">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="20523-113">Além disso:</span><span class="sxs-lookup"><span data-stu-id="20523-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="20523-114">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="20523-115">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="20523-116">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="20523-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="20523-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20523-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="20523-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20523-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20523-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20523-119">Not supported.</span></span> |
| <span data-ttu-id="20523-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20523-120">Application</span></span>                            | <span data-ttu-id="20523-121">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="20523-122">E</span><span class="sxs-lookup"><span data-stu-id="20523-122">And:</span></span><ul><li><span data-ttu-id="20523-123">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="20523-124">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="20523-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="20523-125">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="20523-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="20523-126">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20523-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20523-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20523-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="20523-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20523-128">Request headers</span></span>

| <span data-ttu-id="20523-129">Nome</span><span class="sxs-lookup"><span data-stu-id="20523-129">Name</span></span>          | <span data-ttu-id="20523-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="20523-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20523-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="20523-131">Authorization</span></span> | <span data-ttu-id="20523-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="20523-132">Bearer {token}</span></span> |
| <span data-ttu-id="20523-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20523-133">Content-Type</span></span>  | <span data-ttu-id="20523-134">application/json</span><span class="sxs-lookup"><span data-stu-id="20523-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="20523-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20523-135">Request body</span></span>

<span data-ttu-id="20523-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20523-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20523-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20523-137">Parameter</span></span>    | <span data-ttu-id="20523-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="20523-138">Type</span></span>        | <span data-ttu-id="20523-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="20523-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20523-140">ids</span><span class="sxs-lookup"><span data-stu-id="20523-140">ids</span></span>|<span data-ttu-id="20523-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="20523-141">String collection</span></span>|<span data-ttu-id="20523-142">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="20523-142">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="20523-143">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="20523-143">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="20523-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="20523-144">Response</span></span>

<span data-ttu-id="20523-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto de coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20523-145">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20523-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20523-146">Examples</span></span>

<span data-ttu-id="20523-147">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="20523-147">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="20523-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20523-148">Request</span></span>

<span data-ttu-id="20523-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20523-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20523-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="20523-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="20523-151">C#</span><span class="sxs-lookup"><span data-stu-id="20523-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20523-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20523-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20523-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20523-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20523-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="20523-154">Response</span></span>

<span data-ttu-id="20523-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20523-155">The following is an example of the response.</span></span> 

><span data-ttu-id="20523-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20523-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
