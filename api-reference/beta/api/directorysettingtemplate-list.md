---
title: Listar directorySettingTemplates
description: Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 81b29387cac2ee66aaeab290fb756323122bd1a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861971"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="33c44-104">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="33c44-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c44-105">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="33c44-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="33c44-106">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="33c44-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="33c44-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="33c44-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="33c44-108">A versão/v1.0 dessa API foi renomeada para listar *groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="33c44-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="33c44-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="33c44-109">Permissions</span></span>
<span data-ttu-id="33c44-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c44-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33c44-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33c44-112">Permission type</span></span>      | <span data-ttu-id="33c44-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33c44-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33c44-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33c44-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33c44-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33c44-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33c44-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33c44-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33c44-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33c44-117">Not supported.</span></span>    |
|<span data-ttu-id="33c44-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33c44-118">Application</span></span> | <span data-ttu-id="33c44-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33c44-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33c44-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33c44-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33c44-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33c44-121">Optional query parameters</span></span>
<span data-ttu-id="33c44-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33c44-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33c44-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33c44-123">Request headers</span></span>
| <span data-ttu-id="33c44-124">Nome</span><span class="sxs-lookup"><span data-stu-id="33c44-124">Name</span></span>      |<span data-ttu-id="33c44-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c44-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33c44-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="33c44-126">Authorization</span></span>  | <span data-ttu-id="33c44-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33c44-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33c44-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33c44-129">Request body</span></span>
<span data-ttu-id="33c44-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33c44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33c44-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c44-131">Response</span></span>

<span data-ttu-id="33c44-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33c44-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33c44-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33c44-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33c44-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33c44-134">Request</span></span>
<span data-ttu-id="33c44-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33c44-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33c44-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="33c44-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33c44-137">C#</span><span class="sxs-lookup"><span data-stu-id="33c44-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33c44-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="33c44-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33c44-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33c44-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33c44-140">Java</span><span class="sxs-lookup"><span data-stu-id="33c44-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33c44-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c44-141">Response</span></span>
<span data-ttu-id="33c44-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33c44-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
