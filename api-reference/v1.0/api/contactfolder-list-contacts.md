---
title: Listar contatos
description: Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.
localization_priority: Normal
ms.openlocfilehash: a617cae074ee467d0c47ffcc86351a5e4d65e45a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855465"
---
# <a name="list-contacts"></a><span data-ttu-id="3e374-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="3e374-103">List contacts</span></span>

<span data-ttu-id="3e374-104">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="3e374-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e374-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e374-105">Permissions</span></span>
<span data-ttu-id="3e374-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e374-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e374-108">Permission type</span></span>      | <span data-ttu-id="3e374-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e374-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e374-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e374-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e374-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e374-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e374-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e374-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e374-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e374-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e374-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e374-114">Application</span></span> | <span data-ttu-id="3e374-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e374-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e374-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e374-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e374-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e374-117">Optional query parameters</span></span>
<span data-ttu-id="3e374-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e374-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3e374-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e374-119">Request headers</span></span>
| <span data-ttu-id="3e374-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3e374-120">Name</span></span>       | <span data-ttu-id="3e374-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e374-121">Type</span></span> | <span data-ttu-id="3e374-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e374-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e374-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e374-123">Authorization</span></span>  | <span data-ttu-id="3e374-124">string</span><span class="sxs-lookup"><span data-stu-id="3e374-124">string</span></span>  | <span data-ttu-id="3e374-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e374-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e374-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e374-127">Request body</span></span>
<span data-ttu-id="3e374-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e374-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e374-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e374-129">Response</span></span>

<span data-ttu-id="3e374-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e374-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e374-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e374-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e374-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e374-132">Request</span></span>
<span data-ttu-id="3e374-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e374-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="3e374-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e374-134">Response</span></span>
<span data-ttu-id="3e374-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e374-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "datetime-value",
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
