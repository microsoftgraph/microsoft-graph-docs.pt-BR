---
title: 'usuário: checkMemberObjects'
description: Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 654208a1163e2d99c0685d72588d64d9b0bf228f
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853839"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="68cfa-103">usuário: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="68cfa-103">user: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68cfa-104">Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa para o objeto de usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="68cfa-104">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="68cfa-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="68cfa-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="68cfa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68cfa-106">Permissions</span></span>

<span data-ttu-id="68cfa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68cfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68cfa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68cfa-109">Permission type</span></span>                        | <span data-ttu-id="68cfa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68cfa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68cfa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68cfa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68cfa-112">User. ReadBasic, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="68cfa-113">Além disso:</span><span class="sxs-lookup"><span data-stu-id="68cfa-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="68cfa-114">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="68cfa-115">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="68cfa-116">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="68cfa-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="68cfa-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68cfa-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="68cfa-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68cfa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68cfa-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68cfa-119">Not supported.</span></span> |
| <span data-ttu-id="68cfa-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68cfa-120">Application</span></span>                            | <span data-ttu-id="68cfa-121">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="68cfa-122">E</span><span class="sxs-lookup"><span data-stu-id="68cfa-122">And:</span></span><ul><li><span data-ttu-id="68cfa-123">Se estiver verificando a associação em grupos: Group. Read. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="68cfa-124">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68cfa-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="68cfa-125">Se estiver verificando associação em funções de diretório: RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="68cfa-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="68cfa-126">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cfa-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68cfa-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68cfa-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="68cfa-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68cfa-128">Request headers</span></span>

| <span data-ttu-id="68cfa-129">Nome</span><span class="sxs-lookup"><span data-stu-id="68cfa-129">Name</span></span>          | <span data-ttu-id="68cfa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="68cfa-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68cfa-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="68cfa-131">Authorization</span></span> | <span data-ttu-id="68cfa-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="68cfa-132">Bearer {token}</span></span> |
| <span data-ttu-id="68cfa-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68cfa-133">Content-Type</span></span>  | <span data-ttu-id="68cfa-134">application/json</span><span class="sxs-lookup"><span data-stu-id="68cfa-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="68cfa-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68cfa-135">Request body</span></span>

<span data-ttu-id="68cfa-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68cfa-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68cfa-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="68cfa-137">Parameter</span></span>    | <span data-ttu-id="68cfa-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="68cfa-138">Type</span></span>        | <span data-ttu-id="68cfa-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="68cfa-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68cfa-140">ids</span><span class="sxs-lookup"><span data-stu-id="68cfa-140">ids</span></span>|<span data-ttu-id="68cfa-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="68cfa-141">String collection</span></span>|<span data-ttu-id="68cfa-142">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="68cfa-142">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="68cfa-143">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="68cfa-143">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="68cfa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="68cfa-144">Response</span></span>

<span data-ttu-id="68cfa-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto de coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68cfa-145">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68cfa-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68cfa-146">Examples</span></span>

<span data-ttu-id="68cfa-147">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="68cfa-147">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="68cfa-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68cfa-148">Request</span></span>

<span data-ttu-id="68cfa-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68cfa-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68cfa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="68cfa-150">Response</span></span>

<span data-ttu-id="68cfa-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68cfa-151">The following is an example of the response.</span></span> 

><span data-ttu-id="68cfa-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68cfa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
