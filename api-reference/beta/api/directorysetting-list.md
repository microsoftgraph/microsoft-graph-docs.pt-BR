---
title: Listar configurações de diretório
description: Recupere uma lista de objetos de configuração de diretório.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 740c2c82ba718ed9b99dd1bff229fbabbaf4482c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046598"
---
# <a name="list-directory-settings"></a><span data-ttu-id="d1d8a-103">Listar configurações de diretório</span><span class="sxs-lookup"><span data-stu-id="d1d8a-103">List directory settings</span></span>

<span data-ttu-id="d1d8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1d8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1d8a-105">Recupere uma lista de objetos de configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-105">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="d1d8a-106">**Observação**: a versão /beta dessa API só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-106">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d1d8a-107">A versão /v1.0 dessa API foi renomeada para *List groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-107">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1d8a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1d8a-108">Permissions</span></span>
<span data-ttu-id="d1d8a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1d8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1d8a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1d8a-111">Permission type</span></span>      | <span data-ttu-id="d1d8a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1d8a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1d8a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1d8a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1d8a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1d8a-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1d8a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1d8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1d8a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-116">Not supported.</span></span>    |
|<span data-ttu-id="d1d8a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1d8a-117">Application</span></span> | <span data-ttu-id="d1d8a-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1d8a-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1d8a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d8a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d1d8a-120">Listar configurações de grupo ou de locatário</span><span class="sxs-lookup"><span data-stu-id="d1d8a-120">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1d8a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1d8a-121">Optional query parameters</span></span>
<span data-ttu-id="d1d8a-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1d8a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d8a-123">Request headers</span></span>
| <span data-ttu-id="d1d8a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d1d8a-124">Name</span></span>      |<span data-ttu-id="d1d8a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1d8a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1d8a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1d8a-126">Authorization</span></span>  | <span data-ttu-id="d1d8a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1d8a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d8a-129">Request body</span></span>
<span data-ttu-id="d1d8a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1d8a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d8a-131">Response</span></span>

<span data-ttu-id="d1d8a-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-132">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1d8a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1d8a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1d8a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1d8a-134">Request</span></span>
<span data-ttu-id="d1d8a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1d8a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1d8a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings
```
# <a name="c"></a>[<span data-ttu-id="d1d8a-137">C#</span><span class="sxs-lookup"><span data-stu-id="d1d8a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1d8a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1d8a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1d8a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1d8a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1d8a-140">Java</span><span class="sxs-lookup"><span data-stu-id="d1d8a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d1d8a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1d8a-141">Response</span></span>
<span data-ttu-id="d1d8a-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-142">Here is an example of the response.</span></span> <span data-ttu-id="d1d8a-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d1d8a-143">Note: The response object shown here might be shortened for readability.</span></span>
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
