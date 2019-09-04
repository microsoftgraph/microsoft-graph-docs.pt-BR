---
title: Listar directorySettingTemplates
description: Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a8fbb63327a191ed733c6c2903fb28bde9683e1c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718158"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="0cd0f-104">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="0cd0f-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd0f-105">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="0cd0f-106">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="0cd0f-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0cd0f-108">A versão/v1.0 dessa API foi renomeada para listar *groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd0f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cd0f-109">Permissions</span></span>
<span data-ttu-id="0cd0f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd0f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd0f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cd0f-112">Permission type</span></span>      | <span data-ttu-id="0cd0f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cd0f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd0f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cd0f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0cd0f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cd0f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cd0f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cd0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cd0f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-117">Not supported.</span></span>    |
|<span data-ttu-id="0cd0f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cd0f-118">Application</span></span> | <span data-ttu-id="0cd0f-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd0f-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cd0f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0cd0f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0cd0f-121">Optional query parameters</span></span>
<span data-ttu-id="0cd0f-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cd0f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd0f-123">Request headers</span></span>
| <span data-ttu-id="0cd0f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0cd0f-124">Name</span></span>      |<span data-ttu-id="0cd0f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cd0f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0cd0f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cd0f-126">Authorization</span></span>  | <span data-ttu-id="0cd0f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd0f-129">Request body</span></span>
<span data-ttu-id="0cd0f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd0f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd0f-131">Response</span></span>

<span data-ttu-id="0cd0f-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0cd0f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cd0f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cd0f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd0f-134">Request</span></span>
<span data-ttu-id="0cd0f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0cd0f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd0f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0cd0f-137">C#</span><span class="sxs-lookup"><span data-stu-id="0cd0f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0cd0f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cd0f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0cd0f-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0cd0f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0cd0f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd0f-140">Response</span></span>
<span data-ttu-id="0cd0f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cd0f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
