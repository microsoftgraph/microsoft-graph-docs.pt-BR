---
title: Obter um usuário
description: Recupere as propriedades e os relacionamentos do objeto user.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: cf517326c32a964617e12264079a94ce441413e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815012"
---
# <a name="get-a-user"></a><span data-ttu-id="3850a-103">Obter um usuário</span><span class="sxs-lookup"><span data-stu-id="3850a-103">Get a user</span></span>

> <span data-ttu-id="3850a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3850a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3850a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3850a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3850a-106">Recupere as propriedades e os relacionamentos do objeto user.</span><span class="sxs-lookup"><span data-stu-id="3850a-106">Retrieve the properties and relationships of user object.</span></span>

<span data-ttu-id="3850a-107">Desde que o recurso de **usuário** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **usuário** .</span><span class="sxs-lookup"><span data-stu-id="3850a-107">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="3850a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="3850a-108">Permissions</span></span>
<span data-ttu-id="3850a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3850a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3850a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3850a-111">Permission type</span></span>      | <span data-ttu-id="3850a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3850a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3850a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3850a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3850a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3850a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3850a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3850a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3850a-116">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3850a-116">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="3850a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3850a-117">Application</span></span> | <span data-ttu-id="3850a-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3850a-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3850a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3850a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3850a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3850a-120">Optional query parameters</span></span>
<span data-ttu-id="3850a-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3850a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3850a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3850a-122">Request headers</span></span>
| <span data-ttu-id="3850a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3850a-123">Header</span></span>       | <span data-ttu-id="3850a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3850a-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="3850a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3850a-125">Authorization</span></span>  | <span data-ttu-id="3850a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3850a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3850a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3850a-128">Content-Type</span></span>   | <span data-ttu-id="3850a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3850a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3850a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3850a-130">Request body</span></span>
<span data-ttu-id="3850a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3850a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3850a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3850a-132">Response</span></span>

<span data-ttu-id="3850a-133">Se tiver êxito, este método retorna o código de resposta `200 OK` e o objeto [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3850a-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3850a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3850a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3850a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3850a-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/me
```
##### <a name="response"></a><span data-ttu-id="3850a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3850a-136">Response</span></span>
<span data-ttu-id="3850a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3850a-137">Here is an example of the response.</span></span> <span data-ttu-id="3850a-138">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3850a-138">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="3850a-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="3850a-139">See also</span></span>

- [<span data-ttu-id="3850a-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="3850a-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3850a-141">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="3850a-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3850a-142">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="3850a-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
