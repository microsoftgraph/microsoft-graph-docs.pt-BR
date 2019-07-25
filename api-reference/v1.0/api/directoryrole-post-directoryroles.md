---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd7c199f25f3e2fa324fd49cf46bad93c1cd0901
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865866"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="7ebd2-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="7ebd2-106">Activate directoryRole</span></span>

<span data-ttu-id="7ebd2-p102">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ebd2-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ebd2-111">Permissions</span></span>
<span data-ttu-id="7ebd2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ebd2-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ebd2-114">Permission type</span></span>      | <span data-ttu-id="7ebd2-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ebd2-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7ebd2-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ebd2-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ebd2-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ebd2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ebd2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-119">Not supported.</span></span>    |
|<span data-ttu-id="7ebd2-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-120">Application</span></span> | <span data-ttu-id="7ebd2-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebd2-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ebd2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ebd2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="7ebd2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ebd2-123">Request headers</span></span>
| <span data-ttu-id="7ebd2-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7ebd2-124">Name</span></span>       | <span data-ttu-id="7ebd2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-125">Type</span></span> | <span data-ttu-id="7ebd2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ebd2-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ebd2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ebd2-127">Authorization</span></span>  | <span data-ttu-id="7ebd2-128">string</span><span class="sxs-lookup"><span data-stu-id="7ebd2-128">string</span></span>  | <span data-ttu-id="7ebd2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ebd2-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ebd2-131">Content-Type</span></span>  | <span data-ttu-id="7ebd2-132">string</span><span class="sxs-lookup"><span data-stu-id="7ebd2-132">string</span></span>  | <span data-ttu-id="7ebd2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7ebd2-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ebd2-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ebd2-134">Request body</span></span>
<span data-ttu-id="7ebd2-135">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="7ebd2-136">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="7ebd2-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7ebd2-137">Parameter</span></span> | <span data-ttu-id="7ebd2-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-138">Type</span></span> | <span data-ttu-id="7ebd2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ebd2-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="7ebd2-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="7ebd2-140">roleTemplateId</span></span> | <span data-ttu-id="7ebd2-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ebd2-141">string</span></span> | <span data-ttu-id="7ebd2-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-142">Required.</span></span> <span data-ttu-id="7ebd2-143">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="7ebd2-144">Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="7ebd2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ebd2-145">Response</span></span>

<span data-ttu-id="7ebd2-146">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ebd2-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ebd2-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ebd2-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ebd2-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7ebd2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ebd2-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ebd2-150">C#</span><span class="sxs-lookup"><span data-stu-id="7ebd2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ebd2-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ebd2-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ebd2-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ebd2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7ebd2-153">Java</span><span class="sxs-lookup"><span data-stu-id="7ebd2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7ebd2-154">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7ebd2-154">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7ebd2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ebd2-155">Response</span></span>
<span data-ttu-id="7ebd2-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ebd2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
