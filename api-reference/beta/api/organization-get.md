---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4f0b325100ac8543e51320609e8c4e39ce130fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915449"
---
# <a name="get-organization"></a><span data-ttu-id="fcf34-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="fcf34-103">Get organization</span></span>

> <span data-ttu-id="fcf34-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fcf34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf34-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fcf34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcf34-106">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="fcf34-106">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="fcf34-107">Desde que o recurso de **organização** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância da **organização** .</span><span class="sxs-lookup"><span data-stu-id="fcf34-107">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcf34-108">Permissions</span></span>

<span data-ttu-id="fcf34-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcf34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcf34-111">Permission type</span></span> | <span data-ttu-id="fcf34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcf34-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcf34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcf34-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf34-114">User.Read, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcf34-114">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="fcf34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcf34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcf34-116">Not supported.</span></span> |
|<span data-ttu-id="fcf34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcf34-117">Application</span></span> | <span data-ttu-id="fcf34-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcf34-118">Directory.Read.All</span></span> |

> <span data-ttu-id="fcf34-119">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="fcf34-119">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="fcf34-120">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="fcf34-120">All other properties will return with `null` values.</span></span> <span data-ttu-id="fcf34-121">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="fcf34-121">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="fcf34-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf34-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcf34-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fcf34-123">Optional query parameters</span></span>

<span data-ttu-id="fcf34-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf34-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcf34-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf34-125">Request headers</span></span>

| <span data-ttu-id="fcf34-126">Nome</span><span class="sxs-lookup"><span data-stu-id="fcf34-126">Name</span></span>       | <span data-ttu-id="fcf34-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcf34-127">Type</span></span> | <span data-ttu-id="fcf34-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcf34-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcf34-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcf34-129">Authorization</span></span>  | <span data-ttu-id="fcf34-130">string</span><span class="sxs-lookup"><span data-stu-id="fcf34-130">string</span></span>  | <span data-ttu-id="fcf34-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcf34-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcf34-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf34-133">Request body</span></span>

<span data-ttu-id="fcf34-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcf34-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf34-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf34-135">Response</span></span>

<span data-ttu-id="fcf34-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf34-136">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf34-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcf34-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fcf34-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf34-138">Request</span></span>

<span data-ttu-id="fcf34-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcf34-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="fcf34-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf34-140">Response</span></span>

<span data-ttu-id="fcf34-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcf34-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="fcf34-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="fcf34-144">See also</span></span>

- [<span data-ttu-id="fcf34-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="fcf34-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fcf34-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="fcf34-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
