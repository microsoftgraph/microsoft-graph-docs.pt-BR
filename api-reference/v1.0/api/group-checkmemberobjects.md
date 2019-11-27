---
title: 'Grupo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos ou funções de diretório para o objeto de grupo especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ecfbbdf68501feba69fe4808b8632a7cc04eb09
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621625"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="2cedb-103">Grupo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="2cedb-103">group: checkMemberObjects</span></span>

<span data-ttu-id="2cedb-104">Verifique se há associação em uma lista de grupos ou funções de diretório para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="2cedb-104">Check for membership in a list of groups or directory roles for the specified group.</span></span> <span data-ttu-id="2cedb-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="2cedb-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cedb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2cedb-106">Permissions</span></span>

<span data-ttu-id="2cedb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cedb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cedb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2cedb-109">Permission type</span></span>                        | <span data-ttu-id="2cedb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2cedb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2cedb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2cedb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cedb-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cedb-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="2cedb-113">E</span><span class="sxs-lookup"><span data-stu-id="2cedb-113">And:</span></span><br><ul><li><span data-ttu-id="2cedb-114">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2cedb-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="2cedb-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2cedb-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2cedb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2cedb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cedb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2cedb-117">Not supported.</span></span> |
| <span data-ttu-id="2cedb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2cedb-118">Application</span></span>                            | <span data-ttu-id="2cedb-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cedb-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="2cedb-120">E</span><span class="sxs-lookup"><span data-stu-id="2cedb-120">And:</span></span><br><ul><li><span data-ttu-id="2cedb-121">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2cedb-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="2cedb-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cedb-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cedb-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2cedb-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="2cedb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2cedb-124">Request headers</span></span>

| <span data-ttu-id="2cedb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="2cedb-125">Name</span></span>          | <span data-ttu-id="2cedb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cedb-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2cedb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2cedb-127">Authorization</span></span> | <span data-ttu-id="2cedb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cedb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2cedb-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cedb-130">Content-Type</span></span>  | <span data-ttu-id="2cedb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2cedb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cedb-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2cedb-133">Request body</span></span>

<span data-ttu-id="2cedb-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cedb-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2cedb-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2cedb-135">Parameter</span></span>    | <span data-ttu-id="2cedb-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cedb-136">Type</span></span>        | <span data-ttu-id="2cedb-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cedb-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2cedb-138">ids</span><span class="sxs-lookup"><span data-stu-id="2cedb-138">ids</span></span>|<span data-ttu-id="2cedb-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cedb-139">String collection</span></span>| <span data-ttu-id="2cedb-140">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="2cedb-140">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="2cedb-141">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="2cedb-141">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="2cedb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cedb-142">Response</span></span>

<span data-ttu-id="2cedb-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2cedb-143">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cedb-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2cedb-144">Examples</span></span>

<span data-ttu-id="2cedb-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2cedb-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2cedb-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2cedb-146">Request</span></span>

<span data-ttu-id="2cedb-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2cedb-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2cedb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cedb-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberObjects
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2cedb-149">C#</span><span class="sxs-lookup"><span data-stu-id="2cedb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2cedb-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cedb-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2cedb-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cedb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2cedb-152">Java</span><span class="sxs-lookup"><span data-stu-id="2cedb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2cedb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2cedb-153">Response</span></span>

<span data-ttu-id="2cedb-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2cedb-154">The following is an example of the response.</span></span> 

> <span data-ttu-id="2cedb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2cedb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
