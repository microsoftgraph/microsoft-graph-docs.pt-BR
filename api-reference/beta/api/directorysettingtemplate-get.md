---
title: Obter um modelo de configuração de diretório
description: Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário. Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb79e7de921ef3ed5a67c56b27d07dbc40bc6093
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655786"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="a6c8b-104">Obter um modelo de configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="a6c8b-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c8b-105">Um modelo de configuração de diretório representa um modelo de configurações das quais as configurações podem ser criadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="a6c8b-106">Essa operação permite a recuperação das propriedades do objeto directorySettingTemplate, incluindo as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="a6c8b-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a6c8b-108">A versão do/v1.0 dessa API foi renomeada para *obter groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c8b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6c8b-109">Permissions</span></span>
<span data-ttu-id="a6c8b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c8b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c8b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6c8b-112">Permission type</span></span>      | <span data-ttu-id="a6c8b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6c8b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c8b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6c8b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c8b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6c8b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6c8b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6c8b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c8b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-117">Not supported.</span></span>    |
|<span data-ttu-id="a6c8b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6c8b-118">Application</span></span> | <span data-ttu-id="a6c8b-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c8b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c8b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c8b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6c8b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6c8b-121">Optional query parameters</span></span>
<span data-ttu-id="a6c8b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6c8b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c8b-123">Request headers</span></span>
| <span data-ttu-id="a6c8b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a6c8b-124">Name</span></span>      |<span data-ttu-id="a6c8b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6c8b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6c8b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6c8b-126">Authorization</span></span>  | <span data-ttu-id="a6c8b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c8b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c8b-129">Request body</span></span>
<span data-ttu-id="a6c8b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c8b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c8b-131">Response</span></span>

<span data-ttu-id="a6c8b-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6c8b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6c8b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6c8b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c8b-134">Request</span></span>
<span data-ttu-id="a6c8b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="a6c8b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c8b-136">Response</span></span>
<span data-ttu-id="a6c8b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6c8b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a6c8b-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a6c8b-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a6c8b-141">C#</span><span class="sxs-lookup"><span data-stu-id="a6c8b-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6c8b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6c8b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
