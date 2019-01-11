---
title: Listar contactFolders
description: Obtenha todas as pastas de contato na caixa de correio do usuário conectado.
localization_priority: Normal
ms.openlocfilehash: 17c9cc2328af813fcec2094324310a7e53f61689
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860729"
---
# <a name="list-contactfolders"></a><span data-ttu-id="f5db3-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="f5db3-103">List contactFolders</span></span>

> <span data-ttu-id="f5db3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5db3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5db3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5db3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5db3-106">Obtenha todas as pastas de contato na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f5db3-106">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5db3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f5db3-107">Permissions</span></span>
<span data-ttu-id="f5db3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5db3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5db3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5db3-110">Permission type</span></span>      | <span data-ttu-id="f5db3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5db3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5db3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5db3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5db3-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5db3-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f5db3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5db3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5db3-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5db3-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f5db3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5db3-116">Application</span></span> | <span data-ttu-id="f5db3-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5db3-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5db3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5db3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5db3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5db3-119">Optional query parameters</span></span>
<span data-ttu-id="f5db3-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5db3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5db3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5db3-121">Request headers</span></span>
| <span data-ttu-id="f5db3-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5db3-122">Header</span></span>       | <span data-ttu-id="f5db3-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f5db3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5db3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5db3-124">Authorization</span></span>  | <span data-ttu-id="f5db3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5db3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5db3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5db3-127">Content-Type</span></span>   | <span data-ttu-id="f5db3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f5db3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5db3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5db3-129">Request body</span></span>
<span data-ttu-id="f5db3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5db3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5db3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5db3-131">Response</span></span>

<span data-ttu-id="f5db3-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5db3-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5db3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5db3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5db3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5db3-134">Request</span></span>
<span data-ttu-id="f5db3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5db3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="f5db3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5db3-136">Response</span></span>
<span data-ttu-id="f5db3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5db3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
