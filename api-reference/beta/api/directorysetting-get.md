---
title: Obter uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração de diretório específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e0edc197f1ccb78907a17f56e45c729e0a6136d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324586"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="eed68-103">Obter uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="eed68-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eed68-104">Recupere as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="eed68-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="eed68-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="eed68-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="eed68-106">A versão do/v1.0 dessa API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="eed68-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="eed68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eed68-107">Permissions</span></span>
<span data-ttu-id="eed68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed68-110">Permission type</span></span>      | <span data-ttu-id="eed68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eed68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eed68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eed68-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eed68-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eed68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eed68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed68-115">Not supported.</span></span>    |
|<span data-ttu-id="eed68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eed68-116">Application</span></span> | <span data-ttu-id="eed68-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed68-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eed68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eed68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="eed68-119">Obter uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="eed68-119">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eed68-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eed68-120">Optional query parameters</span></span>
<span data-ttu-id="eed68-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eed68-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eed68-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eed68-122">Request headers</span></span>
| <span data-ttu-id="eed68-123">Nome</span><span class="sxs-lookup"><span data-stu-id="eed68-123">Name</span></span>      |<span data-ttu-id="eed68-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eed68-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eed68-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eed68-125">Authorization</span></span>  | <span data-ttu-id="eed68-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eed68-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed68-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eed68-128">Request body</span></span>
<span data-ttu-id="eed68-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eed68-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eed68-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed68-130">Response</span></span>

<span data-ttu-id="eed68-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eed68-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eed68-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed68-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eed68-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed68-133">Request</span></span>
<span data-ttu-id="eed68-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eed68-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eed68-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eed68-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eed68-136">C#</span><span class="sxs-lookup"><span data-stu-id="eed68-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eed68-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eed68-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eed68-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eed68-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eed68-139">Java</span><span class="sxs-lookup"><span data-stu-id="eed68-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eed68-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed68-140">Response</span></span>
<span data-ttu-id="eed68-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eed68-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
