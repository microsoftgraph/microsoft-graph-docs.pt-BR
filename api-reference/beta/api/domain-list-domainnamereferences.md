---
title: Listar domainNameReferences
description: Recupere uma lista de objetos directoryObject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 082c66367e87ad556cd79fa267eb7dfd8f1e0b56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525763"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="3f84f-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="3f84f-104">List domainNameReferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f84f-p102">Recupere uma lista de objetos [directoryObject](../resources/directoryobject.md) com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="3f84f-p102">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f84f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f84f-107">Permissions</span></span>

<span data-ttu-id="3f84f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f84f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3f84f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f84f-110">Permission type</span></span>      | <span data-ttu-id="3f84f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f84f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f84f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f84f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f84f-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f84f-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="3f84f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f84f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f84f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f84f-115">Not supported.</span></span>    |
|<span data-ttu-id="3f84f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f84f-116">Application</span></span> | <span data-ttu-id="3f84f-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f84f-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f84f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f84f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="3f84f-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="3f84f-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3f84f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f84f-120">Optional query parameters</span></span>

<span data-ttu-id="3f84f-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f84f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f84f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84f-122">Request headers</span></span>

| <span data-ttu-id="3f84f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3f84f-123">Name</span></span>      |<span data-ttu-id="3f84f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f84f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f84f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f84f-125">Authorization</span></span>  | <span data-ttu-id="3f84f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f84f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f84f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84f-128">Request body</span></span>

<span data-ttu-id="3f84f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f84f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f84f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f84f-130">Response</span></span>

<span data-ttu-id="3f84f-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f84f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f84f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f84f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f84f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f84f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="3f84f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f84f-134">Response</span></span>
<span data-ttu-id="3f84f-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f84f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
