---
title: Ativar directoryRole
description: Ative uma função de diretório.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7078b50b05f521d5940cef69565025c5fbf66f21
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854128"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="26509-103">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="26509-103">Activate directoryRole</span></span>

<span data-ttu-id="26509-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26509-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26509-p101">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="26509-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="26509-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="26509-109">Permissions</span></span>
<span data-ttu-id="26509-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26509-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26509-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26509-112">Permission type</span></span>      | <span data-ttu-id="26509-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26509-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26509-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26509-114">Delegated (work or school account)</span></span> | <span data-ttu-id="26509-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26509-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26509-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26509-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26509-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26509-117">Not supported.</span></span>    |
|<span data-ttu-id="26509-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26509-118">Application</span></span> | <span data-ttu-id="26509-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="26509-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="26509-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26509-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="26509-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26509-121">Request headers</span></span>
| <span data-ttu-id="26509-122">Nome</span><span class="sxs-lookup"><span data-stu-id="26509-122">Name</span></span>       | <span data-ttu-id="26509-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="26509-123">Type</span></span> | <span data-ttu-id="26509-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="26509-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26509-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="26509-125">Authorization</span></span>  | <span data-ttu-id="26509-126">string</span><span class="sxs-lookup"><span data-stu-id="26509-126">string</span></span>  | <span data-ttu-id="26509-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26509-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26509-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26509-129">Content-Type</span></span>  | <span data-ttu-id="26509-130">string</span><span class="sxs-lookup"><span data-stu-id="26509-130">string</span></span>  | <span data-ttu-id="26509-131">application/json</span><span class="sxs-lookup"><span data-stu-id="26509-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26509-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26509-132">Request body</span></span>
<span data-ttu-id="26509-133">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="26509-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="26509-134">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="26509-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="26509-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="26509-135">Parameter</span></span> | <span data-ttu-id="26509-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="26509-136">Type</span></span> | <span data-ttu-id="26509-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="26509-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="26509-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="26509-138">roleTemplateId</span></span> | <span data-ttu-id="26509-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26509-139">string</span></span> | <span data-ttu-id="26509-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26509-140">Required.</span></span> <span data-ttu-id="26509-141">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia.</span><span class="sxs-lookup"><span data-stu-id="26509-141">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="26509-142">Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="26509-142">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="26509-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="26509-143">Response</span></span>

<span data-ttu-id="26509-144">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26509-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26509-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26509-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26509-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26509-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="26509-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="26509-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
}
```
# <a name="c"></a>[<span data-ttu-id="26509-148">C#</span><span class="sxs-lookup"><span data-stu-id="26509-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26509-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26509-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26509-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26509-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26509-151">Java</span><span class="sxs-lookup"><span data-stu-id="26509-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="26509-152">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="26509-152">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="26509-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="26509-153">Response</span></span>
<span data-ttu-id="26509-154">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26509-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
  "id": "76f84d30-2759-4c66-915d-65c6e4083fa0",
  "deletedDateTime": null,
  "description": "Can manage all aspects of users and groups, including resetting passwords for limited admins.",
  "displayName": "User Administrator",
  "roleTemplateId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

