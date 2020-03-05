---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b4c94d808185cb056a8481bdfbded071120fe42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434347"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="6e13f-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="6e13f-106">Activate directoryRole</span></span>

<span data-ttu-id="6e13f-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e13f-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e13f-108">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6e13f-108">Activate a directory role.</span></span> <span data-ttu-id="6e13f-109">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="6e13f-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="6e13f-110">Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="6e13f-110">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="6e13f-111">Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="6e13f-111">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e13f-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e13f-112">Permissions</span></span>
<span data-ttu-id="6e13f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e13f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e13f-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e13f-115">Permission type</span></span>      | <span data-ttu-id="6e13f-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e13f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e13f-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e13f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6e13f-118">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6e13f-118">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e13f-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e13f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e13f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e13f-120">Not supported.</span></span>    |
|<span data-ttu-id="6e13f-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e13f-121">Application</span></span> | <span data-ttu-id="6e13f-122">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6e13f-122">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e13f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e13f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="6e13f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e13f-124">Request headers</span></span>
| <span data-ttu-id="6e13f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6e13f-125">Name</span></span>       | <span data-ttu-id="6e13f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e13f-126">Type</span></span> | <span data-ttu-id="6e13f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e13f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e13f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e13f-128">Authorization</span></span>  | <span data-ttu-id="6e13f-129">string</span><span class="sxs-lookup"><span data-stu-id="6e13f-129">string</span></span>  | <span data-ttu-id="6e13f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e13f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e13f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e13f-132">Request body</span></span>
<span data-ttu-id="6e13f-133">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="6e13f-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="6e13f-134">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6e13f-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="6e13f-135">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="6e13f-135">Required parameter</span></span> | <span data-ttu-id="6e13f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e13f-136">Type</span></span> | <span data-ttu-id="6e13f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e13f-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="6e13f-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6e13f-138">roleTemplateId</span></span> | <span data-ttu-id="6e13f-139">string</span><span class="sxs-lookup"><span data-stu-id="6e13f-139">string</span></span> | <span data-ttu-id="6e13f-p105">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e13f-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="6e13f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e13f-142">Response</span></span>

<span data-ttu-id="6e13f-143">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e13f-143">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e13f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e13f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e13f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e13f-145">Request</span></span>
<span data-ttu-id="6e13f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e13f-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e13f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e13f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6e13f-148">C#</span><span class="sxs-lookup"><span data-stu-id="6e13f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e13f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e13f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e13f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e13f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6e13f-151">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="6e13f-151">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6e13f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e13f-152">Response</span></span>
<span data-ttu-id="6e13f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e13f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
