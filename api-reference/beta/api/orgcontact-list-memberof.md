---
title: 'orgContact: membro de lista'
description: Recupere a lista de grupos e unidades administrativas de que o contato é um membro.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c215b13cbce03ef7d12929aeee0af4f2d60403ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525049"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="cb173-103">orgContact: membro de lista</span><span class="sxs-lookup"><span data-stu-id="cb173-103">orgContact: List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb173-104">Recupere a lista de grupos e unidades administrativas de que o contato é um membro.</span><span class="sxs-lookup"><span data-stu-id="cb173-104">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb173-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb173-105">Permissions</span></span>
<span data-ttu-id="cb173-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb173-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb173-108">Permission type</span></span>      | <span data-ttu-id="cb173-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb173-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb173-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb173-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb173-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb173-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb173-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb173-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb173-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb173-113">Not supported.</span></span>    |
|<span data-ttu-id="cb173-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb173-114">Application</span></span> | <span data-ttu-id="cb173-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb173-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb173-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb173-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb173-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb173-117">Optional query parameters</span></span>
<span data-ttu-id="cb173-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb173-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb173-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb173-119">Request headers</span></span>
| <span data-ttu-id="cb173-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cb173-120">Name</span></span>       | <span data-ttu-id="cb173-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb173-121">Type</span></span> | <span data-ttu-id="cb173-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb173-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cb173-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb173-123">Authorization</span></span>  | <span data-ttu-id="cb173-124">string</span><span class="sxs-lookup"><span data-stu-id="cb173-124">string</span></span>  | <span data-ttu-id="cb173-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb173-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb173-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb173-127">Request body</span></span>
<span data-ttu-id="cb173-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb173-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb173-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb173-129">Response</span></span>

<span data-ttu-id="cb173-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb173-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb173-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb173-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb173-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb173-132">Request</span></span>
<span data-ttu-id="cb173-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb173-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="cb173-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb173-134">Response</span></span>
<span data-ttu-id="cb173-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb173-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
