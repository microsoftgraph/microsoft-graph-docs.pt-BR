---
title: Listar contatos
description: Obtenha todos os contatos na caixa de correio do usuário conectado (.../me/contacts) ou a partir da pasta de contato especificada.
ms.openlocfilehash: e15080c9a4d5b0f8e388cc9556ded1ac90ce2823
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034635"
---
# <a name="list-contacts"></a><span data-ttu-id="fe804-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="fe804-103">List contacts</span></span>

> <span data-ttu-id="fe804-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe804-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe804-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe804-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe804-106">Obtenha todos os contatos na caixa de correio do usuário conectado (.../me/contacts) ou a partir da pasta de contato especificada.</span><span class="sxs-lookup"><span data-stu-id="fe804-106">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe804-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="fe804-107">Permissions</span></span>
<span data-ttu-id="fe804-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe804-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe804-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe804-110">Permission type</span></span>      | <span data-ttu-id="fe804-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe804-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe804-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe804-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe804-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe804-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fe804-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe804-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe804-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe804-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fe804-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe804-116">Application</span></span> | <span data-ttu-id="fe804-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe804-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe804-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe804-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe804-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe804-119">Optional query parameters</span></span>
<span data-ttu-id="fe804-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe804-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe804-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe804-121">Request headers</span></span>
| <span data-ttu-id="fe804-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fe804-122">Name</span></span>       | <span data-ttu-id="fe804-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe804-123">Type</span></span> | <span data-ttu-id="fe804-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe804-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe804-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe804-125">Authorization</span></span>  | <span data-ttu-id="fe804-126">string</span><span class="sxs-lookup"><span data-stu-id="fe804-126">string</span></span>  | <span data-ttu-id="fe804-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe804-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe804-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe804-129">Request body</span></span>
<span data-ttu-id="fe804-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe804-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe804-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe804-131">Response</span></span>

<span data-ttu-id="fe804-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe804-132">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe804-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe804-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe804-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe804-134">Request</span></span>
<span data-ttu-id="fe804-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe804-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="fe804-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe804-136">Response</span></span>
<span data-ttu-id="fe804-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe804-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
