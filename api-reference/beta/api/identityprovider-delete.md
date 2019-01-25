---
title: Excluir identityProvider
description: Exclua um identityProvider existente.
localization_priority: Normal
ms.openlocfilehash: bb64f10b656697ab2cf611dd9be0468c295b15e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514352"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="e751f-103">Excluir identityProvider</span><span class="sxs-lookup"><span data-stu-id="e751f-103">Delete identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e751f-104">Exclua um existente [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e751f-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e751f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e751f-105">Permissions</span></span>

<span data-ttu-id="e751f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e751f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e751f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e751f-108">Permission type</span></span>      | <span data-ttu-id="e751f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e751f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e751f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e751f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e751f-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e751f-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e751f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e751f-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e751f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e751f-113">Not supported.</span></span>|
|<span data-ttu-id="e751f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e751f-114">Application</span></span>|<span data-ttu-id="e751f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e751f-115">Not supported.</span></span>|

<span data-ttu-id="e751f-116">A conta do trabalho ou da escola deve ser um administrador global do inquilino.</span><span class="sxs-lookup"><span data-stu-id="e751f-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e751f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e751f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e751f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e751f-118">Request headers</span></span>

|<span data-ttu-id="e751f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e751f-119">Name</span></span>|<span data-ttu-id="e751f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e751f-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e751f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e751f-121">Authorization</span></span>|<span data-ttu-id="e751f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e751f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e751f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e751f-124">Request body</span></span>

<span data-ttu-id="e751f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e751f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e751f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e751f-126">Response</span></span>

<span data-ttu-id="e751f-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e751f-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e751f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e751f-128">Example</span></span>

<span data-ttu-id="e751f-129">O exemplo a seguir exclui uma **identityProvider**.</span><span class="sxs-lookup"><span data-stu-id="e751f-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e751f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e751f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e751f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e751f-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
