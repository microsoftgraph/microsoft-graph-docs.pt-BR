---
title: Configurações de grupo de lista
description: Recupere uma lista de objetos de configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9540bc3083187fe26885582230b365a4d80603ad
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613501"
---
# <a name="list-group-settings"></a><span data-ttu-id="62ef0-103">Configurações de grupo de lista</span><span class="sxs-lookup"><span data-stu-id="62ef0-103">List group settings</span></span>

<span data-ttu-id="62ef0-104">Recupere uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="62ef0-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="62ef0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62ef0-105">Permissions</span></span>

<span data-ttu-id="62ef0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62ef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="62ef0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62ef0-108">Permission type</span></span>      | <span data-ttu-id="62ef0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62ef0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62ef0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62ef0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62ef0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62ef0-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62ef0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62ef0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62ef0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62ef0-113">Not supported.</span></span>    |
|<span data-ttu-id="62ef0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62ef0-114">Application</span></span> | <span data-ttu-id="62ef0-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62ef0-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62ef0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62ef0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="62ef0-117">Listar configurações de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="62ef0-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="62ef0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62ef0-118">Optional query parameters</span></span>
<span data-ttu-id="62ef0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62ef0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="62ef0-120">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="62ef0-120">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62ef0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62ef0-121">Request headers</span></span>
| <span data-ttu-id="62ef0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="62ef0-122">Name</span></span> | <span data-ttu-id="62ef0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ef0-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="62ef0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62ef0-124">Authorization</span></span>  | <span data-ttu-id="62ef0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62ef0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62ef0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62ef0-127">Request body</span></span>
<span data-ttu-id="62ef0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62ef0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62ef0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62ef0-129">Response</span></span>

<span data-ttu-id="62ef0-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62ef0-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62ef0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62ef0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="62ef0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62ef0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="62ef0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="62ef0-133">Response</span></span>

<span data-ttu-id="62ef0-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62ef0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62ef0-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="62ef0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62ef0-137">Basic</span><span class="sxs-lookup"><span data-stu-id="62ef0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62ef0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62ef0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsettings-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
