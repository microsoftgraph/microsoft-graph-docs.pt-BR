---
title: Obter uma configuração de diretório
description: Recupere as propriedades de um objeto de configuração de diretório específico.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a31a3d647bf00a5a827ea43f6ecda1950f5221f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956216"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="aaf1f-103">Obter uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="aaf1f-103">Get a directory setting</span></span>

<span data-ttu-id="aaf1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaf1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaf1f-105">Recupere as propriedades de um objeto de configuração de diretório específico.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="aaf1f-106">**Observação** : a versão do/beta desta API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-106">**Note** : The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="aaf1f-107">A versão do/v1.0 dessa API foi renomeada para *obter groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaf1f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="aaf1f-108">Permissions</span></span>
<span data-ttu-id="aaf1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaf1f-111">Permission type</span></span>      | <span data-ttu-id="aaf1f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaf1f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaf1f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaf1f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aaf1f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aaf1f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aaf1f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaf1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaf1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-116">Not supported.</span></span>    |
|<span data-ttu-id="aaf1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaf1f-117">Application</span></span> | <span data-ttu-id="aaf1f-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf1f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaf1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaf1f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="aaf1f-120">Obter uma configuração específica de todo o locatário ou grupo</span><span class="sxs-lookup"><span data-stu-id="aaf1f-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aaf1f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aaf1f-121">Optional query parameters</span></span>
<span data-ttu-id="aaf1f-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaf1f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf1f-123">Request headers</span></span>
| <span data-ttu-id="aaf1f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="aaf1f-124">Name</span></span>      |<span data-ttu-id="aaf1f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaf1f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaf1f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaf1f-126">Authorization</span></span>  | <span data-ttu-id="aaf1f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf1f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf1f-129">Request body</span></span>
<span data-ttu-id="aaf1f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaf1f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf1f-131">Response</span></span>

<span data-ttu-id="aaf1f-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aaf1f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaf1f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aaf1f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf1f-134">Request</span></span>
<span data-ttu-id="aaf1f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aaf1f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaf1f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="aaf1f-137">C#</span><span class="sxs-lookup"><span data-stu-id="aaf1f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaf1f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaf1f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaf1f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaf1f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaf1f-140">Java</span><span class="sxs-lookup"><span data-stu-id="aaf1f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aaf1f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf1f-141">Response</span></span>
<span data-ttu-id="aaf1f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaf1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
