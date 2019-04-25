---
title: 'orgContact: obter gerente'
description: Obter o gerente do contato
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96833e9b38b2d988a3843e097a11fe38a247c0b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539798"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="3bbb4-103">orgContact: obter gerente</span><span class="sxs-lookup"><span data-stu-id="3bbb4-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bbb4-104">Obter o gerente do contato</span><span class="sxs-lookup"><span data-stu-id="3bbb4-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="3bbb4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bbb4-105">Permissions</span></span>
<span data-ttu-id="3bbb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bbb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bbb4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bbb4-108">Permission type</span></span>      | <span data-ttu-id="3bbb4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bbb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bbb4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bbb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bbb4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bbb4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bbb4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bbb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bbb4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-113">Not supported.</span></span>    |
|<span data-ttu-id="3bbb4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bbb4-114">Application</span></span> | <span data-ttu-id="3bbb4-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bbb4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bbb4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bbb4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bbb4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bbb4-117">Optional query parameters</span></span>
<span data-ttu-id="3bbb4-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bbb4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbb4-119">Request headers</span></span>
| <span data-ttu-id="3bbb4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3bbb4-120">Name</span></span>       | <span data-ttu-id="3bbb4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bbb4-121">Type</span></span> | <span data-ttu-id="3bbb4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bbb4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3bbb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bbb4-123">Authorization</span></span>  | <span data-ttu-id="3bbb4-124">string</span><span class="sxs-lookup"><span data-stu-id="3bbb4-124">string</span></span>  | <span data-ttu-id="3bbb4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bbb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbb4-127">Request body</span></span>
<span data-ttu-id="3bbb4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bbb4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbb4-129">Response</span></span>

<span data-ttu-id="3bbb4-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3bbb4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bbb4-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3bbb4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbb4-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="3bbb4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbb4-133">Response</span></span>

<span data-ttu-id="3bbb4-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bbb4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
