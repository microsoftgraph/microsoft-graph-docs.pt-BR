---
title: Listar directorySettingTemplates
description: Essa operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 06b62e868991f7da1012b23fbacc940665cd8350
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046542"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="7dbc4-103">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="7dbc4-103">List directorySettingTemplates</span></span>

<span data-ttu-id="7dbc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dbc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dbc4-105">Os modelos de configuração de diretório representam um conjunto de modelos de configurações de diretório, a partir dos quais as configurações de diretório podem ser criadas e usadas em um locatário.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="7dbc4-106">Essa operação recupera a lista de objetos **directorySettingTemplates** disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-106">This operation retrieves the list of available **directorySettingTemplates** objects.</span></span>

> <span data-ttu-id="7dbc4-107">**Observação**: a versão /beta dessa API só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7dbc4-108">A versão /v1.0 desta API foi renomeada para *List groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dbc4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dbc4-109">Permissions</span></span>
<span data-ttu-id="7dbc4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dbc4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dbc4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dbc4-112">Permission type</span></span>      | <span data-ttu-id="7dbc4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dbc4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dbc4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dbc4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7dbc4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dbc4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7dbc4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dbc4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dbc4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-117">Not supported.</span></span>    |
|<span data-ttu-id="7dbc4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dbc4-118">Application</span></span> | <span data-ttu-id="7dbc4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbc4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dbc4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dbc4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7dbc4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dbc4-121">Optional query parameters</span></span>
<span data-ttu-id="7dbc4-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dbc4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc4-123">Request headers</span></span>
| <span data-ttu-id="7dbc4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7dbc4-124">Name</span></span>      |<span data-ttu-id="7dbc4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dbc4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7dbc4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dbc4-126">Authorization</span></span>  | <span data-ttu-id="7dbc4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dbc4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc4-129">Request body</span></span>
<span data-ttu-id="7dbc4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dbc4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbc4-131">Response</span></span>

<span data-ttu-id="7dbc4-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7dbc4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dbc4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7dbc4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbc4-134">Request</span></span>
<span data-ttu-id="7dbc4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dbc4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dbc4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="7dbc4-137">C#</span><span class="sxs-lookup"><span data-stu-id="7dbc4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dbc4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dbc4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dbc4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dbc4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dbc4-140">Java</span><span class="sxs-lookup"><span data-stu-id="7dbc4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7dbc4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbc4-141">Response</span></span>
<span data-ttu-id="7dbc4-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-142">Here is an example of the response.</span></span> <span data-ttu-id="7dbc4-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-143">Note: The response object shown here might be shortened for readability.</span></span>
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


