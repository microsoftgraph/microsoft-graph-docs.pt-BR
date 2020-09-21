---
title: 'usuário: checkMemberObjects'
description: Verifique se há associação em uma lista de funções de grupo ou de diretório para o objeto de usuário especificado.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e0450d4bdb35978fcb1f7b375babd6900f11b88d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967748"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="8ac5c-103">usuário: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8ac5c-103">user: checkMemberObjects</span></span>

<span data-ttu-id="8ac5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ac5c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ac5c-105">Verifique se há associação em uma lista de funções de grupo ou de diretório para o objeto de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="8ac5c-106">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ac5c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ac5c-107">Permissions</span></span>

<span data-ttu-id="8ac5c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ac5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ac5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ac5c-110">Permission type</span></span>                        | <span data-ttu-id="8ac5c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ac5c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ac5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ac5c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ac5c-113">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="8ac5c-114">Além disso:</span><span class="sxs-lookup"><span data-stu-id="8ac5c-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="8ac5c-115">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="8ac5c-116">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="8ac5c-117">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8ac5c-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="8ac5c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="8ac5c-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ac5c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ac5c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-120">Not supported.</span></span> |
| <span data-ttu-id="8ac5c-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ac5c-121">Application</span></span>                            | <span data-ttu-id="8ac5c-122">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="8ac5c-123">E</span><span class="sxs-lookup"><span data-stu-id="8ac5c-123">And:</span></span><ul><li><span data-ttu-id="8ac5c-124">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="8ac5c-125">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="8ac5c-126">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8ac5c-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="8ac5c-127">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ac5c-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ac5c-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ac5c-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="8ac5c-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5c-129">Request headers</span></span>

| <span data-ttu-id="8ac5c-130">Nome</span><span class="sxs-lookup"><span data-stu-id="8ac5c-130">Name</span></span>          | <span data-ttu-id="8ac5c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ac5c-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ac5c-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ac5c-132">Authorization</span></span> | <span data-ttu-id="8ac5c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ac5c-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ac5c-135">Content-Type</span></span>  | <span data-ttu-id="8ac5c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ac5c-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5c-138">Request body</span></span>

<span data-ttu-id="8ac5c-139">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ac5c-140">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8ac5c-140">Parameter</span></span>    | <span data-ttu-id="8ac5c-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ac5c-141">Type</span></span>        | <span data-ttu-id="8ac5c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ac5c-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ac5c-143">ids</span><span class="sxs-lookup"><span data-stu-id="8ac5c-143">ids</span></span>|<span data-ttu-id="8ac5c-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ac5c-144">String collection</span></span>|<span data-ttu-id="8ac5c-145">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-145">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="8ac5c-146">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-146">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="8ac5c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac5c-147">Response</span></span>

<span data-ttu-id="8ac5c-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto de coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-148">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ac5c-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ac5c-149">Examples</span></span>

<span data-ttu-id="8ac5c-150">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-150">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8ac5c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ac5c-151">Request</span></span>

<span data-ttu-id="8ac5c-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ac5c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ac5c-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
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
# <a name="c"></a>[<span data-ttu-id="8ac5c-154">C#</span><span class="sxs-lookup"><span data-stu-id="8ac5c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ac5c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ac5c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ac5c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ac5c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ac5c-157">Java</span><span class="sxs-lookup"><span data-stu-id="8ac5c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ac5c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ac5c-158">Response</span></span>

<span data-ttu-id="8ac5c-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-159">The following is an example of the response.</span></span> 

><span data-ttu-id="8ac5c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ac5c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

