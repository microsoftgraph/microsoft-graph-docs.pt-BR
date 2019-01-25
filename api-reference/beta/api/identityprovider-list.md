---
title: Lista identityProviders
description: Recupere todos os identityProviders no diretório.
localization_priority: Normal
ms.openlocfilehash: 4226e6f091527d2df8bfb544327ec2e49f2b890c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529730"
---
# <a name="list-identityproviders"></a><span data-ttu-id="6f6b7-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="6f6b7-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f6b7-104">Recupere todos os [identityProviders](../resources/identityprovider.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f6b7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f6b7-105">Permissions</span></span>

<span data-ttu-id="6f6b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6b7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f6b7-108">Permission type</span></span>      | <span data-ttu-id="6f6b7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f6b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6b7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f6b7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6f6b7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6b7-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6f6b7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f6b7-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6f6b7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-113">Not supported.</span></span>|
|<span data-ttu-id="6f6b7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6b7-114">Application</span></span>|<span data-ttu-id="6f6b7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-115">Not supported.</span></span>|

<span data-ttu-id="6f6b7-116">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="6f6b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f6b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="6f6b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6b7-118">Request headers</span></span>

|<span data-ttu-id="6f6b7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6f6b7-119">Name</span></span>|<span data-ttu-id="6f6b7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f6b7-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6f6b7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f6b7-121">Authorization</span></span>|<span data-ttu-id="6f6b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6b7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6b7-124">Request body</span></span>

<span data-ttu-id="6f6b7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f6b7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6b7-126">Response</span></span>

<span data-ttu-id="6f6b7-127">Se tiver êxito, este método retornará `200 OK` código de resposta e uma coleção de [identityProviders](../resources/identityprovider.md) na representação JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6b7-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f6b7-128">Example</span></span>

<span data-ttu-id="6f6b7-129">O exemplo a seguir recupera todos os **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="6f6b7-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="6f6b7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6b7-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="6f6b7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6b7-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
