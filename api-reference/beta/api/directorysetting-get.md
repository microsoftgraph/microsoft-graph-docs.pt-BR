---
title: Obter uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração de diretório específico.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 839a21f1afaa2667f40e4328a066f82e5d3b025c
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312824"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="25cc1-103">Obter uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="25cc1-103">Get a directory setting</span></span>

<span data-ttu-id="25cc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25cc1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cc1-105">Recupere as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="25cc1-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="25cc1-106">**Observação**: a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="25cc1-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="25cc1-107">A versão do/v1.0 dessa API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="25cc1-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="25cc1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="25cc1-108">Permissions</span></span>
<span data-ttu-id="25cc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25cc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25cc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25cc1-111">Permission type</span></span>      | <span data-ttu-id="25cc1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25cc1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25cc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25cc1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="25cc1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="25cc1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25cc1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25cc1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25cc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25cc1-116">Not supported.</span></span>    |
|<span data-ttu-id="25cc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25cc1-117">Application</span></span> | <span data-ttu-id="25cc1-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25cc1-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25cc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25cc1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="25cc1-120">Obter uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="25cc1-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25cc1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25cc1-121">Optional query parameters</span></span>
<span data-ttu-id="25cc1-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25cc1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25cc1-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc1-123">Request headers</span></span>
| <span data-ttu-id="25cc1-124">Nome</span><span class="sxs-lookup"><span data-stu-id="25cc1-124">Name</span></span>      |<span data-ttu-id="25cc1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="25cc1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25cc1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="25cc1-126">Authorization</span></span>  | <span data-ttu-id="25cc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25cc1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25cc1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc1-129">Request body</span></span>
<span data-ttu-id="25cc1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25cc1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25cc1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cc1-131">Response</span></span>

<span data-ttu-id="25cc1-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25cc1-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25cc1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25cc1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25cc1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25cc1-134">Request</span></span>
<span data-ttu-id="25cc1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25cc1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25cc1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="25cc1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="25cc1-137">C#</span><span class="sxs-lookup"><span data-stu-id="25cc1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25cc1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25cc1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25cc1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25cc1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="25cc1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="25cc1-140">Response</span></span>
<span data-ttu-id="25cc1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25cc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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