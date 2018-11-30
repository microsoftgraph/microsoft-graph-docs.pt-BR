---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
ms.openlocfilehash: 34cf72acda93ec8cbd6362512edf57f09d50dc7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006141"
---
# <a name="get-organization"></a><span data-ttu-id="d769b-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="d769b-103">Get organization</span></span>

<span data-ttu-id="d769b-104">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="d769b-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="d769b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d769b-105">Permissions</span></span>
<span data-ttu-id="d769b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d769b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d769b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d769b-108">Permission type</span></span>      | <span data-ttu-id="d769b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d769b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d769b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d769b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d769b-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d769b-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="d769b-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d769b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d769b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d769b-113">Not supported.</span></span>    |
|<span data-ttu-id="d769b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d769b-114">Application</span></span> | <span data-ttu-id="d769b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d769b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d769b-116">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="d769b-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="d769b-117">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="d769b-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="d769b-118">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="d769b-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="d769b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d769b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d769b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d769b-120">Optional query parameters</span></span>
<span data-ttu-id="d769b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d769b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d769b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d769b-122">Request headers</span></span>
| <span data-ttu-id="d769b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d769b-123">Name</span></span>       | <span data-ttu-id="d769b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d769b-124">Type</span></span> | <span data-ttu-id="d769b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d769b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d769b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d769b-126">Authorization</span></span>  | <span data-ttu-id="d769b-127">string</span><span class="sxs-lookup"><span data-stu-id="d769b-127">string</span></span>  | <span data-ttu-id="d769b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d769b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d769b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d769b-130">Request body</span></span>
<span data-ttu-id="d769b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d769b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d769b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d769b-132">Response</span></span>

<span data-ttu-id="d769b-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d769b-133">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d769b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d769b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d769b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d769b-135">Request</span></span>
<span data-ttu-id="d769b-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d769b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="d769b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d769b-137">Response</span></span>
<span data-ttu-id="d769b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d769b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->