---
title: Listar directorySettingTemplates
description: Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adfb303e24b637af4b77ac9f3cfd357ca09ece8f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655779"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="a2392-104">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="a2392-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2392-105">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="a2392-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="a2392-106">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a2392-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="a2392-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="a2392-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a2392-108">A versão/v1.0 dessa API foi renomeada para listar *groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="a2392-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2392-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2392-109">Permissions</span></span>
<span data-ttu-id="a2392-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2392-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2392-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2392-112">Permission type</span></span>      | <span data-ttu-id="a2392-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2392-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2392-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2392-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a2392-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2392-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2392-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2392-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2392-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2392-117">Not supported.</span></span>    |
|<span data-ttu-id="a2392-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2392-118">Application</span></span> | <span data-ttu-id="a2392-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2392-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2392-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2392-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2392-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2392-121">Optional query parameters</span></span>
<span data-ttu-id="a2392-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2392-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2392-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2392-123">Request headers</span></span>
| <span data-ttu-id="a2392-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a2392-124">Name</span></span>      |<span data-ttu-id="a2392-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2392-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2392-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2392-126">Authorization</span></span>  | <span data-ttu-id="a2392-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2392-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2392-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2392-129">Request body</span></span>
<span data-ttu-id="a2392-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2392-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2392-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2392-131">Response</span></span>

<span data-ttu-id="a2392-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2392-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2392-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2392-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2392-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2392-134">Request</span></span>
<span data-ttu-id="a2392-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2392-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="a2392-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2392-136">Response</span></span>
<span data-ttu-id="a2392-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2392-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
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
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2392-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a2392-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2392-141">C#</span><span class="sxs-lookup"><span data-stu-id="a2392-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2392-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2392-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
