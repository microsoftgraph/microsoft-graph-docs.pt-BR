---
title: Obter identityProvider
description: Recupere as propriedades de um identityprovider existente.
localization_priority: Normal
ms.openlocfilehash: 8315c43bcd99b9ea96b408cd2feb61a59369e4c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501333"
---
# <a name="get-identityprovider"></a><span data-ttu-id="e89b6-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="e89b6-103">Get identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e89b6-104">Recuperar as propriedades de um [identityProvider](../resources/identityprovider.md) existente.</span><span class="sxs-lookup"><span data-stu-id="e89b6-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e89b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e89b6-105">Permissions</span></span>

<span data-ttu-id="e89b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e89b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e89b6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e89b6-108">Permission type</span></span>      | <span data-ttu-id="e89b6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e89b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e89b6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e89b6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e89b6-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e89b6-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e89b6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e89b6-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e89b6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e89b6-113">Not supported.</span></span>|
|<span data-ttu-id="e89b6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e89b6-114">Application</span></span>|<span data-ttu-id="e89b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e89b6-115">Not supported.</span></span>|

<span data-ttu-id="e89b6-116">A conta corporativa ou de estudante deve ser um administrador global do locatário.</span><span class="sxs-lookup"><span data-stu-id="e89b6-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e89b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e89b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e89b6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e89b6-118">Request headers</span></span>

|<span data-ttu-id="e89b6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e89b6-119">Name</span></span>|<span data-ttu-id="e89b6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e89b6-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e89b6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e89b6-121">Authorization</span></span>|<span data-ttu-id="e89b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e89b6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e89b6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e89b6-124">Request body</span></span>

<span data-ttu-id="e89b6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e89b6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e89b6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e89b6-126">Response</span></span>

<span data-ttu-id="e89b6-127">Se bem-sucedido, esse método retornará `200 OK` código de resposta e uma representação JSON do [identityProvider](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e89b6-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89b6-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e89b6-128">Example</span></span>

<span data-ttu-id="e89b6-129">O exemplo a seguir recupera uma determinada **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e89b6-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e89b6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e89b6-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e89b6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e89b6-131">Response</span></span>

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
