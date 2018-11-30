---
title: Listar organização
description: Recupere uma lista de objetos de organização.
ms.openlocfilehash: 01a6b08b241fcf28edc9b387a00693acfa7beb71
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040025"
---
# <a name="list-organization"></a><span data-ttu-id="711e8-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="711e8-103">List organization</span></span>

> <span data-ttu-id="711e8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="711e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="711e8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="711e8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="711e8-106">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="711e8-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="711e8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="711e8-107">Permissions</span></span>
<span data-ttu-id="711e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="711e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="711e8-110">Permission type</span></span>      | <span data-ttu-id="711e8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="711e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="711e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="711e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="711e8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="711e8-113">Not supported.</span></span>    |
|<span data-ttu-id="711e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="711e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="711e8-115">Not supported.</span></span>    |
|<span data-ttu-id="711e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="711e8-116">Application</span></span> | <span data-ttu-id="711e8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="711e8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="711e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="711e8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="711e8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="711e8-119">Optional query parameters</span></span>
<span data-ttu-id="711e8-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="711e8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="711e8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="711e8-121">Request headers</span></span>
| <span data-ttu-id="711e8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="711e8-122">Name</span></span>       | <span data-ttu-id="711e8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="711e8-123">Type</span></span> | <span data-ttu-id="711e8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="711e8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="711e8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="711e8-125">Authorization</span></span>  | <span data-ttu-id="711e8-126">string</span><span class="sxs-lookup"><span data-stu-id="711e8-126">string</span></span>  | <span data-ttu-id="711e8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="711e8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="711e8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="711e8-129">Request body</span></span>
<span data-ttu-id="711e8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="711e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="711e8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="711e8-131">Response</span></span>

<span data-ttu-id="711e8-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="711e8-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="711e8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="711e8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="711e8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="711e8-134">Request</span></span>
<span data-ttu-id="711e8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="711e8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="711e8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="711e8-136">Response</span></span>
<span data-ttu-id="711e8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="711e8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->