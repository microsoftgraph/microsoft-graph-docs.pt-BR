---
title: Listar configurações de diretório
description: Recupere uma lista de objetos de configuração de diretório.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2704340a0f6366329bae9074e0e0d206146333e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319451"
---
# <a name="list-directory-settings"></a><span data-ttu-id="d55f9-103">Listar configurações de diretório</span><span class="sxs-lookup"><span data-stu-id="d55f9-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d55f9-104">Recupere uma lista de objetos de configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="d55f9-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="d55f9-105">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="d55f9-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d55f9-106">A versão/v1.0 dessa API foi renomeada para listar *groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="d55f9-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d55f9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d55f9-107">Permissions</span></span>
<span data-ttu-id="d55f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d55f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d55f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d55f9-110">Permission type</span></span>      | <span data-ttu-id="d55f9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d55f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d55f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d55f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d55f9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d55f9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d55f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d55f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d55f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d55f9-115">Not supported.</span></span>    |
|<span data-ttu-id="d55f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d55f9-116">Application</span></span> | <span data-ttu-id="d55f9-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55f9-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d55f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d55f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d55f9-119">Listar configurações de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="d55f9-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d55f9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d55f9-120">Optional query parameters</span></span>
<span data-ttu-id="d55f9-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d55f9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d55f9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d55f9-122">Request headers</span></span>
| <span data-ttu-id="d55f9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d55f9-123">Name</span></span>      |<span data-ttu-id="d55f9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d55f9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d55f9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d55f9-125">Authorization</span></span>  | <span data-ttu-id="d55f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d55f9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d55f9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d55f9-128">Request body</span></span>
<span data-ttu-id="d55f9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d55f9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d55f9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d55f9-130">Response</span></span>

<span data-ttu-id="d55f9-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d55f9-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d55f9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d55f9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d55f9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d55f9-133">Request</span></span>
<span data-ttu-id="d55f9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d55f9-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d55f9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d55f9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d55f9-136">C#</span><span class="sxs-lookup"><span data-stu-id="d55f9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d55f9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d55f9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d55f9-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d55f9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d55f9-139">Java</span><span class="sxs-lookup"><span data-stu-id="d55f9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d55f9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d55f9-140">Response</span></span>
<span data-ttu-id="d55f9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d55f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
