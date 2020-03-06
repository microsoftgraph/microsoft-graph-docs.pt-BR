---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ada6d1aba533ad8eeabbd4cbf64046f130711ff4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517927"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="54339-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="54339-106">Activate directoryRole</span></span>

<span data-ttu-id="54339-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54339-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54339-p102">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="54339-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="54339-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="54339-112">Permissions</span></span>
<span data-ttu-id="54339-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54339-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54339-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54339-115">Permission type</span></span>      | <span data-ttu-id="54339-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54339-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54339-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54339-117">Delegated (work or school account)</span></span> | <span data-ttu-id="54339-118">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="54339-118">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54339-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54339-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54339-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54339-120">Not supported.</span></span>    |
|<span data-ttu-id="54339-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54339-121">Application</span></span> | <span data-ttu-id="54339-122">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="54339-122">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="54339-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54339-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="54339-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54339-124">Request headers</span></span>
| <span data-ttu-id="54339-125">Nome</span><span class="sxs-lookup"><span data-stu-id="54339-125">Name</span></span>       | <span data-ttu-id="54339-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="54339-126">Type</span></span> | <span data-ttu-id="54339-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="54339-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="54339-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="54339-128">Authorization</span></span>  | <span data-ttu-id="54339-129">string</span><span class="sxs-lookup"><span data-stu-id="54339-129">string</span></span>  | <span data-ttu-id="54339-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54339-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54339-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54339-132">Content-Type</span></span>  | <span data-ttu-id="54339-133">string</span><span class="sxs-lookup"><span data-stu-id="54339-133">string</span></span>  | <span data-ttu-id="54339-134">application/json</span><span class="sxs-lookup"><span data-stu-id="54339-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54339-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54339-135">Request body</span></span>
<span data-ttu-id="54339-136">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="54339-136">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="54339-137">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="54339-137">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="54339-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="54339-138">Parameter</span></span> | <span data-ttu-id="54339-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="54339-139">Type</span></span> | <span data-ttu-id="54339-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="54339-140">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="54339-141">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="54339-141">roleTemplateId</span></span> | <span data-ttu-id="54339-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54339-142">string</span></span> | <span data-ttu-id="54339-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54339-143">Required.</span></span> <span data-ttu-id="54339-144">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia.</span><span class="sxs-lookup"><span data-stu-id="54339-144">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="54339-145">Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="54339-145">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="54339-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="54339-146">Response</span></span>

<span data-ttu-id="54339-147">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54339-147">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54339-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54339-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54339-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54339-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54339-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="54339-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="54339-151">C#</span><span class="sxs-lookup"><span data-stu-id="54339-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54339-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54339-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54339-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54339-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54339-154">Java</span><span class="sxs-lookup"><span data-stu-id="54339-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="54339-155">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="54339-155">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="54339-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="54339-156">Response</span></span>
<span data-ttu-id="54339-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54339-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
