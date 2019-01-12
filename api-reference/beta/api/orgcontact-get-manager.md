---
title: 'orgContact: Get manager'
description: Obtenha o gerente do contato
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b660fabfe03d6e34897375f7f36470774f95450
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942889"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="2df8b-103">orgContact: Get manager</span><span class="sxs-lookup"><span data-stu-id="2df8b-103">orgContact: Get manager</span></span>

> <span data-ttu-id="2df8b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2df8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2df8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2df8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2df8b-106">Obtenha o gerente do contato</span><span class="sxs-lookup"><span data-stu-id="2df8b-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="2df8b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2df8b-107">Permissions</span></span>
<span data-ttu-id="2df8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df8b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df8b-110">Permission type</span></span>      | <span data-ttu-id="2df8b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2df8b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2df8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df8b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2df8b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2df8b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2df8b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df8b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2df8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df8b-115">Not supported.</span></span>    |
|<span data-ttu-id="2df8b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df8b-116">Application</span></span> | <span data-ttu-id="2df8b-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df8b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2df8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df8b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2df8b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2df8b-119">Optional query parameters</span></span>
<span data-ttu-id="2df8b-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2df8b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8b-121">Request headers</span></span>
| <span data-ttu-id="2df8b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2df8b-122">Name</span></span>       | <span data-ttu-id="2df8b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df8b-123">Type</span></span> | <span data-ttu-id="2df8b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df8b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2df8b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df8b-125">Authorization</span></span>  | <span data-ttu-id="2df8b-126">string</span><span class="sxs-lookup"><span data-stu-id="2df8b-126">string</span></span>  | <span data-ttu-id="2df8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df8b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2df8b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8b-129">Request body</span></span>
<span data-ttu-id="2df8b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2df8b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df8b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8b-131">Response</span></span>

<span data-ttu-id="2df8b-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df8b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2df8b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df8b-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2df8b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df8b-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="2df8b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df8b-135">Response</span></span>

<span data-ttu-id="2df8b-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2df8b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
