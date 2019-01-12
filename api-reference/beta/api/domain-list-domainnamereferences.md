---
title: Listar domainNameReferences
description: Recupere uma lista de objetos directoryObject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a0e2cdbfb4a7a0899650e884a190ea45855d72c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985365"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="650ce-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="650ce-104">List domainNameReferences</span></span>

> <span data-ttu-id="650ce-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="650ce-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="650ce-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="650ce-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="650ce-p103">Recupere uma lista de objetos [directoryObject](../resources/directoryobject.md) com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="650ce-p103">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="650ce-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="650ce-109">Permissions</span></span>

<span data-ttu-id="650ce-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="650ce-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="650ce-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="650ce-112">Permission type</span></span>      | <span data-ttu-id="650ce-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="650ce-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="650ce-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="650ce-114">Delegated (work or school account)</span></span> | <span data-ttu-id="650ce-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="650ce-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="650ce-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="650ce-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="650ce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="650ce-117">Not supported.</span></span>    |
|<span data-ttu-id="650ce-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="650ce-118">Application</span></span> | <span data-ttu-id="650ce-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="650ce-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="650ce-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="650ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="650ce-121">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="650ce-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="650ce-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="650ce-122">Optional query parameters</span></span>

<span data-ttu-id="650ce-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="650ce-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="650ce-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="650ce-124">Request headers</span></span>

| <span data-ttu-id="650ce-125">Nome</span><span class="sxs-lookup"><span data-stu-id="650ce-125">Name</span></span>      |<span data-ttu-id="650ce-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="650ce-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="650ce-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="650ce-127">Authorization</span></span>  | <span data-ttu-id="650ce-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="650ce-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="650ce-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="650ce-130">Request body</span></span>

<span data-ttu-id="650ce-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="650ce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="650ce-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="650ce-132">Response</span></span>

<span data-ttu-id="650ce-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="650ce-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="650ce-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="650ce-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="650ce-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="650ce-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="650ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="650ce-136">Response</span></span>
<span data-ttu-id="650ce-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="650ce-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
