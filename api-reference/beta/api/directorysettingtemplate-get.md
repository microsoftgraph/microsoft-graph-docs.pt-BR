---
title: Obter um modelo de configuração de diretório
description: Permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9e9622eccff2cedfb8085790fd4b7d44b140944
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956125"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="2a808-103">Obter um modelo de configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="2a808-103">Get a directory setting template</span></span>

<span data-ttu-id="2a808-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a808-105">Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="2a808-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="2a808-106">Essa operação permite a recuperação das propriedades do objeto **directorySettingTemplate** , incluindo as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="2a808-106">This operation allows retrieval of the properties of the **directorySettingTemplate** object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="2a808-107">**Observação** : a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="2a808-107">**Note** : The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="2a808-108">A versão do/v1.0 dessa API foi renomeada para *obter groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="2a808-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a808-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a808-109">Permissions</span></span>
<span data-ttu-id="2a808-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a808-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a808-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a808-112">Permission type</span></span>      | <span data-ttu-id="2a808-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a808-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a808-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a808-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2a808-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a808-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a808-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a808-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a808-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a808-117">Not supported.</span></span>    |
|<span data-ttu-id="2a808-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a808-118">Application</span></span> | <span data-ttu-id="2a808-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a808-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a808-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a808-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a808-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a808-121">Optional query parameters</span></span>
<span data-ttu-id="2a808-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a808-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a808-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a808-123">Request headers</span></span>
| <span data-ttu-id="2a808-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2a808-124">Name</span></span>      |<span data-ttu-id="2a808-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a808-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a808-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a808-126">Authorization</span></span>  | <span data-ttu-id="2a808-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a808-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a808-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a808-129">Request body</span></span>
<span data-ttu-id="2a808-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a808-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a808-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a808-131">Response</span></span>

<span data-ttu-id="2a808-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a808-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a808-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a808-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a808-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a808-134">Request</span></span>
<span data-ttu-id="2a808-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a808-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a808-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a808-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="2a808-137">C#</span><span class="sxs-lookup"><span data-stu-id="2a808-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a808-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a808-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a808-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a808-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a808-140">Java</span><span class="sxs-lookup"><span data-stu-id="2a808-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2a808-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a808-141">Response</span></span>
<span data-ttu-id="2a808-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a808-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


