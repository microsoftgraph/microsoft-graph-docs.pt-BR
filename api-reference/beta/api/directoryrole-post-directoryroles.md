---
title: Ativar directoryRole
description: Ative uma função de diretório.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5078af3f13fdee8f2d7603d700b19e62530f6f72
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046780"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="1e7a0-103">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="1e7a0-103">Activate directoryRole</span></span>

<span data-ttu-id="1e7a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e7a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e7a0-105">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-105">Activate a directory role.</span></span> <span data-ttu-id="1e7a0-106">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="1e7a0-107">Somente os Administradores da Empresa e as funções implícitas de diretório Usuários são ativados por padrão.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-107">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="1e7a0-108">Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="1e7a0-108">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e7a0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e7a0-109">Permissions</span></span>
<span data-ttu-id="1e7a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e7a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e7a0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e7a0-112">Permission type</span></span>      | <span data-ttu-id="1e7a0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e7a0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e7a0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e7a0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1e7a0-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e7a0-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e7a0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e7a0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e7a0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-117">Not supported.</span></span>    |
|<span data-ttu-id="1e7a0-118">Application</span><span class="sxs-lookup"><span data-stu-id="1e7a0-118">Application</span></span> | <span data-ttu-id="1e7a0-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="1e7a0-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e7a0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e7a0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="1e7a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e7a0-121">Request headers</span></span>
| <span data-ttu-id="1e7a0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1e7a0-122">Name</span></span>       | <span data-ttu-id="1e7a0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e7a0-123">Type</span></span> | <span data-ttu-id="1e7a0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e7a0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e7a0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e7a0-125">Authorization</span></span>  | <span data-ttu-id="1e7a0-126">string</span><span class="sxs-lookup"><span data-stu-id="1e7a0-126">string</span></span>  | <span data-ttu-id="1e7a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e7a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e7a0-129">Request body</span></span>
<span data-ttu-id="1e7a0-130">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="1e7a0-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="1e7a0-131">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="1e7a0-132">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="1e7a0-132">Required parameter</span></span> | <span data-ttu-id="1e7a0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e7a0-133">Type</span></span> | <span data-ttu-id="1e7a0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e7a0-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="1e7a0-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="1e7a0-135">roleTemplateId</span></span> | <span data-ttu-id="1e7a0-136">string</span><span class="sxs-lookup"><span data-stu-id="1e7a0-136">string</span></span> | <span data-ttu-id="1e7a0-p104">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="1e7a0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e7a0-139">Response</span></span>

<span data-ttu-id="1e7a0-140">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-140">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e7a0-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e7a0-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e7a0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e7a0-142">Request</span></span>
<span data-ttu-id="1e7a0-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e7a0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e7a0-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1e7a0-145">C#</span><span class="sxs-lookup"><span data-stu-id="1e7a0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e7a0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e7a0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e7a0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e7a0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e7a0-148">Java</span><span class="sxs-lookup"><span data-stu-id="1e7a0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1e7a0-149">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="1e7a0-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1e7a0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e7a0-150">Response</span></span>
<span data-ttu-id="1e7a0-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-151">Here is an example of the response.</span></span> <span data-ttu-id="1e7a0-152">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1e7a0-152">Note: The response object shown here might be shortened for readability.</span></span>
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


