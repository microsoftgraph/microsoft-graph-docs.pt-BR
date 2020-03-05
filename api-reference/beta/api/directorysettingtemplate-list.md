---
title: Listar directorySettingTemplates
description: Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.  Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ff5c102652d0c04bf37c3545b50fe320071be07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433829"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="7ccf4-104">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="7ccf4-104">List directorySettingTemplates</span></span>

<span data-ttu-id="7ccf4-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ccf4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ccf4-106">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-106">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="7ccf4-107">Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-107">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="7ccf4-108">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-108">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7ccf4-109">A versão/v1.0 dessa API foi renomeada para *listar groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-109">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ccf4-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ccf4-110">Permissions</span></span>
<span data-ttu-id="7ccf4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ccf4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ccf4-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ccf4-113">Permission type</span></span>      | <span data-ttu-id="7ccf4-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ccf4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ccf4-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ccf4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7ccf4-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ccf4-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ccf4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ccf4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ccf4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-118">Not supported.</span></span>    |
|<span data-ttu-id="7ccf4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ccf4-119">Application</span></span> | <span data-ttu-id="7ccf4-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ccf4-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ccf4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ccf4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ccf4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ccf4-122">Optional query parameters</span></span>
<span data-ttu-id="7ccf4-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ccf4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccf4-124">Request headers</span></span>
| <span data-ttu-id="7ccf4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="7ccf4-125">Name</span></span>      |<span data-ttu-id="7ccf4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ccf4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ccf4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ccf4-127">Authorization</span></span>  | <span data-ttu-id="7ccf4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ccf4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccf4-130">Request body</span></span>
<span data-ttu-id="7ccf4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ccf4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ccf4-132">Response</span></span>

<span data-ttu-id="7ccf4-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-133">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ccf4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ccf4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ccf4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ccf4-135">Request</span></span>
<span data-ttu-id="7ccf4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ccf4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ccf4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="7ccf4-138">C#</span><span class="sxs-lookup"><span data-stu-id="7ccf4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ccf4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ccf4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ccf4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ccf4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7ccf4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ccf4-141">Response</span></span>
<span data-ttu-id="7ccf4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ccf4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
