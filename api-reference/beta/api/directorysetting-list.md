---
title: Listar configurações de diretório
description: Recupere uma lista de objetos de configuração de diretório.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0b105d5bd4c5178b3a9f62aeda781bdb74eae3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375633"
---
# <a name="list-directory-settings"></a><span data-ttu-id="17d82-103">Listar configurações de diretório</span><span class="sxs-lookup"><span data-stu-id="17d82-103">List directory settings</span></span>

<span data-ttu-id="17d82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17d82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d82-105">Recupere uma lista de objetos de configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="17d82-105">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="17d82-106">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="17d82-106">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="17d82-107">A versão/v1.0 dessa API foi renomeada para *listar groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="17d82-107">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="17d82-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="17d82-108">Permissions</span></span>
<span data-ttu-id="17d82-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17d82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d82-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17d82-111">Permission type</span></span>      | <span data-ttu-id="17d82-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17d82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17d82-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17d82-113">Delegated (work or school account)</span></span> | <span data-ttu-id="17d82-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17d82-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17d82-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17d82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d82-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17d82-116">Not supported.</span></span>    |
|<span data-ttu-id="17d82-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17d82-117">Application</span></span> | <span data-ttu-id="17d82-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d82-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17d82-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17d82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="17d82-120">Listar configurações de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="17d82-120">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17d82-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17d82-121">Optional query parameters</span></span>
<span data-ttu-id="17d82-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17d82-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17d82-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17d82-123">Request headers</span></span>
| <span data-ttu-id="17d82-124">Nome</span><span class="sxs-lookup"><span data-stu-id="17d82-124">Name</span></span>      |<span data-ttu-id="17d82-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d82-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17d82-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="17d82-126">Authorization</span></span>  | <span data-ttu-id="17d82-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d82-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17d82-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17d82-129">Request body</span></span>
<span data-ttu-id="17d82-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17d82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d82-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d82-131">Response</span></span>

<span data-ttu-id="17d82-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17d82-132">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17d82-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17d82-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17d82-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17d82-134">Request</span></span>
<span data-ttu-id="17d82-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17d82-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17d82-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="17d82-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings
```
# <a name="c"></a>[<span data-ttu-id="17d82-137">C#</span><span class="sxs-lookup"><span data-stu-id="17d82-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17d82-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17d82-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17d82-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17d82-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17d82-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d82-140">Response</span></span>
<span data-ttu-id="17d82-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17d82-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
