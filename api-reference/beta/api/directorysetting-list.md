---
title: Listar configurações de diretório
description: Recupere uma lista de objetos de configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 609515db8eb40523ab3c861818e98b327fee36c7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417182"
---
# <a name="list-directory-settings"></a><span data-ttu-id="b6dc1-103">Listar configurações de diretório</span><span class="sxs-lookup"><span data-stu-id="b6dc1-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6dc1-104">Recupere uma lista de objetos de configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="b6dc1-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b6dc1-106">A versão/v1.0 dessa API foi renomeada para listar *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6dc1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6dc1-107">Permissions</span></span>
<span data-ttu-id="b6dc1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6dc1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6dc1-110">Permission type</span></span>      | <span data-ttu-id="b6dc1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6dc1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6dc1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6dc1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6dc1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6dc1-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6dc1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6dc1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6dc1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-115">Not supported.</span></span>    |
|<span data-ttu-id="b6dc1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6dc1-116">Application</span></span> | <span data-ttu-id="b6dc1-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6dc1-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6dc1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6dc1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b6dc1-119">Listar configurações de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="b6dc1-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6dc1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6dc1-120">Optional query parameters</span></span>
<span data-ttu-id="b6dc1-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6dc1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6dc1-122">Request headers</span></span>
| <span data-ttu-id="b6dc1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b6dc1-123">Name</span></span>      |<span data-ttu-id="b6dc1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6dc1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6dc1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6dc1-125">Authorization</span></span>  | <span data-ttu-id="b6dc1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6dc1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6dc1-128">Request body</span></span>
<span data-ttu-id="b6dc1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6dc1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6dc1-130">Response</span></span>

<span data-ttu-id="b6dc1-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6dc1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6dc1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6dc1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6dc1-133">Request</span></span>
<span data-ttu-id="b6dc1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b6dc1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6dc1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b6dc1-136">C#</span><span class="sxs-lookup"><span data-stu-id="b6dc1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6dc1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6dc1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b6dc1-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b6dc1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6dc1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6dc1-139">Response</span></span>
<span data-ttu-id="b6dc1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6dc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
