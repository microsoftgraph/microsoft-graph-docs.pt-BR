---
title: Obter um modelo de configuração de diretório
description: Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário. Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c648064f182453c3ffeccad885b7cba44ebb6de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433836"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="b6cf8-104">Obter um modelo de configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="b6cf8-104">Get a directory setting template</span></span>

<span data-ttu-id="b6cf8-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6cf8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6cf8-106">Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-106">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="b6cf8-107">Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-107">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="b6cf8-108">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-108">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b6cf8-109">A versão do/v1.0 dessa API foi renomeada para *obter groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-109">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6cf8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6cf8-110">Permissions</span></span>
<span data-ttu-id="b6cf8-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6cf8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6cf8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6cf8-113">Permission type</span></span>      | <span data-ttu-id="b6cf8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6cf8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6cf8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6cf8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b6cf8-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6cf8-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6cf8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6cf8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6cf8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-118">Not supported.</span></span>    |
|<span data-ttu-id="b6cf8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6cf8-119">Application</span></span> | <span data-ttu-id="b6cf8-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6cf8-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6cf8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cf8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6cf8-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6cf8-122">Optional query parameters</span></span>
<span data-ttu-id="b6cf8-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6cf8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cf8-124">Request headers</span></span>
| <span data-ttu-id="b6cf8-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b6cf8-125">Name</span></span>      |<span data-ttu-id="b6cf8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6cf8-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6cf8-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6cf8-127">Authorization</span></span>  | <span data-ttu-id="b6cf8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6cf8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cf8-130">Request body</span></span>
<span data-ttu-id="b6cf8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6cf8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cf8-132">Response</span></span>

<span data-ttu-id="b6cf8-133">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-133">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6cf8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6cf8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6cf8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6cf8-135">Request</span></span>
<span data-ttu-id="b6cf8-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6cf8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6cf8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="b6cf8-138">C#</span><span class="sxs-lookup"><span data-stu-id="b6cf8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6cf8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6cf8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6cf8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6cf8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6cf8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6cf8-141">Response</span></span>
<span data-ttu-id="b6cf8-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6cf8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

{
  "id": "id-value",
  "displayName": "displayName-value",
  "description": "description-value",
  "values": [
    {
      "name": "name-value",
      "type": "type-value",
      "defaultValue": "defaultValue-value",
      "description": "description-value"
    }
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
