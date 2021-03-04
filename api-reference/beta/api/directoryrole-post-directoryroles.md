---
title: Ativar directoryRole
description: Ative uma função de diretório.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aa9a2d1a5f174ada043215e7ae6ba55e81a3473a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436747"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="a2034-103">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="a2034-103">Activate directoryRole</span></span>

<span data-ttu-id="a2034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2034-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2034-105">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a2034-105">Activate a directory role.</span></span> <span data-ttu-id="a2034-106">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="a2034-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="a2034-107">Somente os Administradores da Empresa e as funções implícitas de diretório Usuários são ativados por padrão.</span><span class="sxs-lookup"><span data-stu-id="a2034-107">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="a2034-108">Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="a2034-108">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2034-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2034-109">Permissions</span></span>
<span data-ttu-id="a2034-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2034-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2034-112">Permission type</span></span>      | <span data-ttu-id="a2034-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2034-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2034-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2034-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a2034-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2034-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2034-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2034-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2034-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2034-117">Not supported.</span></span>    |
|<span data-ttu-id="a2034-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2034-118">Application</span></span> | <span data-ttu-id="a2034-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a2034-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2034-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2034-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="a2034-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2034-121">Request headers</span></span>
| <span data-ttu-id="a2034-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a2034-122">Name</span></span>       | <span data-ttu-id="a2034-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2034-123">Type</span></span> | <span data-ttu-id="a2034-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2034-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2034-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2034-125">Authorization</span></span>  | <span data-ttu-id="a2034-126">string</span><span class="sxs-lookup"><span data-stu-id="a2034-126">string</span></span>  | <span data-ttu-id="a2034-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2034-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2034-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2034-129">Request body</span></span>
<span data-ttu-id="a2034-130">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a2034-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="a2034-131">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a2034-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="a2034-132">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="a2034-132">Required parameter</span></span> | <span data-ttu-id="a2034-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2034-133">Type</span></span> | <span data-ttu-id="a2034-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2034-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="a2034-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a2034-135">roleTemplateId</span></span> | <span data-ttu-id="a2034-136">string</span><span class="sxs-lookup"><span data-stu-id="a2034-136">string</span></span> | <span data-ttu-id="a2034-p104">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2034-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="a2034-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2034-139">Response</span></span>

<span data-ttu-id="a2034-140">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2034-140">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2034-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2034-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2034-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2034-142">Request</span></span>
<span data-ttu-id="a2034-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2034-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2034-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2034-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2034-145">C#</span><span class="sxs-lookup"><span data-stu-id="a2034-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2034-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2034-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2034-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2034-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2034-148">Java</span><span class="sxs-lookup"><span data-stu-id="a2034-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a2034-149">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a2034-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a2034-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2034-150">Response</span></span>
<span data-ttu-id="a2034-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2034-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


