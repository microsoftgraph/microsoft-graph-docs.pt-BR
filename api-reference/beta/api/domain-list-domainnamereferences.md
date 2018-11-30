---
title: Listar domainNameReferences
description: Recupere uma lista de objetos directoryObject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.
ms.openlocfilehash: 145fbf3221467d4802a93f4f5112b49eaa99b339
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035882"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="88d1c-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="88d1c-104">List domainNameReferences</span></span>

> <span data-ttu-id="88d1c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="88d1c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88d1c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="88d1c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88d1c-p103">Recupere uma lista de objetos [directoryObject](../resources/directoryobject.md) com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="88d1c-p103">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="88d1c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="88d1c-109">Permissions</span></span>

<span data-ttu-id="88d1c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d1c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88d1c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88d1c-112">Permission type</span></span>      | <span data-ttu-id="88d1c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88d1c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d1c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88d1c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="88d1c-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d1c-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="88d1c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88d1c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d1c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88d1c-117">Not supported.</span></span>    |
|<span data-ttu-id="88d1c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88d1c-118">Application</span></span> | <span data-ttu-id="88d1c-119">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d1c-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88d1c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88d1c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="88d1c-121">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="88d1c-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="88d1c-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88d1c-122">Optional query parameters</span></span>

<span data-ttu-id="88d1c-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88d1c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88d1c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88d1c-124">Request headers</span></span>

| <span data-ttu-id="88d1c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="88d1c-125">Name</span></span>      |<span data-ttu-id="88d1c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d1c-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88d1c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="88d1c-127">Authorization</span></span>  | <span data-ttu-id="88d1c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88d1c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88d1c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88d1c-130">Request body</span></span>

<span data-ttu-id="88d1c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88d1c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d1c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d1c-132">Response</span></span>

<span data-ttu-id="88d1c-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88d1c-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88d1c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88d1c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88d1c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88d1c-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="88d1c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d1c-136">Response</span></span>
<span data-ttu-id="88d1c-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88d1c-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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