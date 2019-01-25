---
title: Obter identityProvider
description: Recupere as propriedades de um identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: 8315c43bcd99b9ea96b408cd2feb61a59369e4c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523068"
---
# <a name="get-identityprovider"></a><span data-ttu-id="d4b57-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="d4b57-103">Get identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b57-104">Recupere as propriedades de um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="d4b57-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b57-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4b57-105">Permissions</span></span>

<span data-ttu-id="d4b57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4b57-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4b57-108">Permission type</span></span>      | <span data-ttu-id="d4b57-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4b57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4b57-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4b57-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d4b57-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b57-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d4b57-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4b57-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d4b57-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4b57-113">Not supported.</span></span>|
|<span data-ttu-id="d4b57-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4b57-114">Application</span></span>|<span data-ttu-id="d4b57-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4b57-115">Not supported.</span></span>|

<span data-ttu-id="d4b57-116">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="d4b57-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4b57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b57-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d4b57-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b57-118">Request headers</span></span>

|<span data-ttu-id="d4b57-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d4b57-119">Name</span></span>|<span data-ttu-id="d4b57-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4b57-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d4b57-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4b57-121">Authorization</span></span>|<span data-ttu-id="d4b57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4b57-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b57-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b57-124">Request body</span></span>

<span data-ttu-id="d4b57-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4b57-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b57-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b57-126">Response</span></span>

<span data-ttu-id="d4b57-127">Se tiver êxito, este método retornará `200 OK` código de resposta e uma representação de JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4b57-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4b57-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4b57-128">Example</span></span>

<span data-ttu-id="d4b57-129">O exemplo a seguir recupera um específicos **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="d4b57-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="d4b57-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b57-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="d4b57-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b57-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
