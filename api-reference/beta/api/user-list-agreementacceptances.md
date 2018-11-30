---
title: Lista agreementAcceptances
description: Recupere uma lista de objetos de agreementAcceptance de um usuário.
ms.openlocfilehash: 77e10ff9e35db37247f91f4c473c1775c295033a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040283"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="a9223-103">Lista agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="a9223-103">List agreementAcceptances</span></span>

> <span data-ttu-id="a9223-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9223-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9223-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9223-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9223-106">Recupere uma lista de objetos de [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a9223-106">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9223-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a9223-107">Permissions</span></span>
<span data-ttu-id="a9223-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9223-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9223-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9223-110">Permission type</span></span>                        | <span data-ttu-id="a9223-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9223-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9223-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9223-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9223-113">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="a9223-113">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="a9223-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9223-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9223-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9223-115">Not supported.</span></span> |
|<span data-ttu-id="a9223-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9223-116">Application</span></span>                            | <span data-ttu-id="a9223-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9223-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9223-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9223-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="a9223-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9223-119">Request headers</span></span>
| <span data-ttu-id="a9223-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a9223-120">Name</span></span>      |<span data-ttu-id="a9223-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9223-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9223-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9223-122">Authorization</span></span> | <span data-ttu-id="a9223-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a9223-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9223-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9223-124">Request body</span></span>
<span data-ttu-id="a9223-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9223-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a9223-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9223-126">Response</span></span>
<span data-ttu-id="a9223-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9223-127">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9223-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9223-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9223-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9223-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="a9223-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9223-130">Response</span></span>
><span data-ttu-id="a9223-p103">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9223-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
