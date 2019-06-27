---
title: Obter uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração de diretório específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 386f65388b690f30ea6e2065530f1e5a0aff316c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260575"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="a0ea3-103">Obter uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="a0ea3-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ea3-104">Recupere as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="a0ea3-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a0ea3-106">A versão do/v1.0 dessa API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ea3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0ea3-107">Permissions</span></span>
<span data-ttu-id="a0ea3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ea3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0ea3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0ea3-110">Permission type</span></span>      | <span data-ttu-id="a0ea3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0ea3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0ea3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0ea3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0ea3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0ea3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0ea3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0ea3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ea3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-115">Not supported.</span></span>    |
|<span data-ttu-id="a0ea3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ea3-116">Application</span></span> | <span data-ttu-id="a0ea3-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0ea3-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ea3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ea3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a0ea3-119">Obter uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="a0ea3-119">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0ea3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0ea3-120">Optional query parameters</span></span>
<span data-ttu-id="a0ea3-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0ea3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ea3-122">Request headers</span></span>
| <span data-ttu-id="a0ea3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a0ea3-123">Name</span></span>      |<span data-ttu-id="a0ea3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ea3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0ea3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0ea3-125">Authorization</span></span>  | <span data-ttu-id="a0ea3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0ea3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ea3-128">Request body</span></span>
<span data-ttu-id="a0ea3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0ea3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ea3-130">Response</span></span>

<span data-ttu-id="a0ea3-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0ea3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0ea3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0ea3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ea3-133">Request</span></span>
<span data-ttu-id="a0ea3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="a0ea3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ea3-135">Response</span></span>
<span data-ttu-id="a0ea3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0ea3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0ea3-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a0ea3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0ea3-140">C#</span><span class="sxs-lookup"><span data-stu-id="a0ea3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0ea3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0ea3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a0ea3-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a0ea3-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directorysetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
