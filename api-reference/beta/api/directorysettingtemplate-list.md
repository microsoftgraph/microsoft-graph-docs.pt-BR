---
title: Listar directorySettingTemplates
description: Esta operação recupera a lista de objetos directorySettingTemplates disponíveis.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 09afd3ff60f9f9d12a94ad52c8a7e6dcf34935cf
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180155"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="e8af5-103">Listar directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="e8af5-103">List directorySettingTemplates</span></span>

<span data-ttu-id="e8af5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8af5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8af5-105">Modelos de configuração de diretório representa um conjunto de modelos de configurações de diretório, de onde as configurações de diretório podem ser criadas e usadas dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="e8af5-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="e8af5-106">Esta operação recupera a lista de objetos **directorySettingTemplates** disponíveis.</span><span class="sxs-lookup"><span data-stu-id="e8af5-106">This operation retrieves the list of available **directorySettingTemplates** objects.</span></span>

> <span data-ttu-id="e8af5-107">**Observação**: a versão do/beta dessa API só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="e8af5-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="e8af5-108">A versão/v1.0 dessa API foi renomeada para *listar groupSettingTemplate*.</span><span class="sxs-lookup"><span data-stu-id="e8af5-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8af5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8af5-109">Permissions</span></span>
<span data-ttu-id="e8af5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8af5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8af5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8af5-112">Permission type</span></span>      | <span data-ttu-id="e8af5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8af5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8af5-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8af5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e8af5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8af5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8af5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8af5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8af5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8af5-117">Not supported.</span></span>    |
|<span data-ttu-id="e8af5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8af5-118">Application</span></span> | <span data-ttu-id="e8af5-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8af5-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8af5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8af5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8af5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8af5-121">Optional query parameters</span></span>
<span data-ttu-id="e8af5-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8af5-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8af5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8af5-123">Request headers</span></span>
| <span data-ttu-id="e8af5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e8af5-124">Name</span></span>      |<span data-ttu-id="e8af5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8af5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8af5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8af5-126">Authorization</span></span>  | <span data-ttu-id="e8af5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8af5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8af5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8af5-129">Request body</span></span>
<span data-ttu-id="e8af5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8af5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8af5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8af5-131">Response</span></span>

<span data-ttu-id="e8af5-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [directorySettingTemplate](../resources/directorysettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8af5-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8af5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8af5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8af5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8af5-134">Request</span></span>
<span data-ttu-id="e8af5-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8af5-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8af5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8af5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="e8af5-137">C#</span><span class="sxs-lookup"><span data-stu-id="e8af5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8af5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8af5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8af5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8af5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8af5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8af5-140">Response</span></span>
<span data-ttu-id="e8af5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8af5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
