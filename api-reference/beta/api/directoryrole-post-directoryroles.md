---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 10689fa2902dc53aa3a3246aafb9bd923d5d2e89
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260673"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="a8e85-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="a8e85-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8e85-107">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8e85-107">Activate a directory role.</span></span> <span data-ttu-id="a8e85-108">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="a8e85-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="a8e85-109">Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="a8e85-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="a8e85-110">Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="a8e85-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8e85-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8e85-111">Permissions</span></span>
<span data-ttu-id="a8e85-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e85-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e85-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8e85-114">Permission type</span></span>      | <span data-ttu-id="a8e85-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8e85-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8e85-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8e85-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a8e85-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8e85-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8e85-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8e85-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8e85-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8e85-119">Not supported.</span></span>    |
|<span data-ttu-id="a8e85-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8e85-120">Application</span></span> | <span data-ttu-id="a8e85-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e85-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8e85-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e85-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="a8e85-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e85-123">Request headers</span></span>
| <span data-ttu-id="a8e85-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a8e85-124">Name</span></span>       | <span data-ttu-id="a8e85-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e85-125">Type</span></span> | <span data-ttu-id="a8e85-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e85-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8e85-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8e85-127">Authorization</span></span>  | <span data-ttu-id="a8e85-128">string</span><span class="sxs-lookup"><span data-stu-id="a8e85-128">string</span></span>  | <span data-ttu-id="a8e85-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8e85-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8e85-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e85-131">Request body</span></span>
<span data-ttu-id="a8e85-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a8e85-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="a8e85-133">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a8e85-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="a8e85-134">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="a8e85-134">Required parameter</span></span> | <span data-ttu-id="a8e85-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e85-135">Type</span></span> | <span data-ttu-id="a8e85-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e85-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="a8e85-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a8e85-137">roleTemplateId</span></span> | <span data-ttu-id="a8e85-138">string</span><span class="sxs-lookup"><span data-stu-id="a8e85-138">string</span></span> | <span data-ttu-id="a8e85-p105">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e85-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="a8e85-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e85-141">Response</span></span>

<span data-ttu-id="a8e85-142">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e85-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e85-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8e85-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8e85-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e85-144">Request</span></span>
<span data-ttu-id="a8e85-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e85-145">Here is an example of the request.</span></span>
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
<span data-ttu-id="a8e85-146">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a8e85-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a8e85-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e85-147">Response</span></span>
<span data-ttu-id="a8e85-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8e85-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a8e85-151">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a8e85-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a8e85-152">C#</span><span class="sxs-lookup"><span data-stu-id="a8e85-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8e85-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8e85-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a8e85-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a8e85-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
