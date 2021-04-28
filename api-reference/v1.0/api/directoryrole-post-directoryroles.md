---
title: Ativar directoryRole
description: Ative uma função de diretório.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6295e6d60d35eb434e1e5b1d91dae3fc60eda84f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050518"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="7de3e-103">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="7de3e-103">Activate directoryRole</span></span>

<span data-ttu-id="7de3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7de3e-p101">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="7de3e-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="7de3e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7de3e-109">Permissions</span></span>
<span data-ttu-id="7de3e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7de3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7de3e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7de3e-112">Permission type</span></span>      | <span data-ttu-id="7de3e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7de3e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7de3e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7de3e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7de3e-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7de3e-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7de3e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7de3e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7de3e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7de3e-117">Not supported.</span></span>    |
|<span data-ttu-id="7de3e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7de3e-118">Application</span></span> | <span data-ttu-id="7de3e-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="7de3e-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="7de3e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7de3e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="7de3e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7de3e-121">Request headers</span></span>
| <span data-ttu-id="7de3e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7de3e-122">Name</span></span>       | <span data-ttu-id="7de3e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7de3e-123">Type</span></span> | <span data-ttu-id="7de3e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de3e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7de3e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7de3e-125">Authorization</span></span>  | <span data-ttu-id="7de3e-126">string</span><span class="sxs-lookup"><span data-stu-id="7de3e-126">string</span></span>  | <span data-ttu-id="7de3e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7de3e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7de3e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7de3e-129">Content-Type</span></span>  | <span data-ttu-id="7de3e-130">string</span><span class="sxs-lookup"><span data-stu-id="7de3e-130">string</span></span>  | <span data-ttu-id="7de3e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="7de3e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7de3e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7de3e-132">Request body</span></span>
<span data-ttu-id="7de3e-133">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7de3e-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="7de3e-134">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7de3e-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="7de3e-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7de3e-135">Parameter</span></span> | <span data-ttu-id="7de3e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="7de3e-136">Type</span></span> | <span data-ttu-id="7de3e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7de3e-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="7de3e-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="7de3e-138">roleTemplateId</span></span> | <span data-ttu-id="7de3e-139">string</span><span class="sxs-lookup"><span data-stu-id="7de3e-139">string</span></span> | <span data-ttu-id="7de3e-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7de3e-140">Required.</span></span> <span data-ttu-id="7de3e-141">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia.</span><span class="sxs-lookup"><span data-stu-id="7de3e-141">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="7de3e-142">Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7de3e-142">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="7de3e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de3e-143">Response</span></span>

<span data-ttu-id="7de3e-144">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7de3e-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7de3e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7de3e-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7de3e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7de3e-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7de3e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7de3e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7de3e-148">C#</span><span class="sxs-lookup"><span data-stu-id="7de3e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7de3e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7de3e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7de3e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7de3e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7de3e-151">Java</span><span class="sxs-lookup"><span data-stu-id="7de3e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7de3e-152">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7de3e-152">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7de3e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7de3e-153">Response</span></span>
<span data-ttu-id="7de3e-154">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7de3e-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
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

