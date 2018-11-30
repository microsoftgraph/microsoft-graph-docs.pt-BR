---
title: Obter sectionGroup
description: Recupere as propriedades e os relacionamentos de um objeto sectionGroup.
ms.openlocfilehash: 12ba258056ae1a317541e01b6747e8de5a97450f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040012"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="4ab56-103">Obter sectionGroup</span><span class="sxs-lookup"><span data-stu-id="4ab56-103">Get sectionGroup</span></span>

> <span data-ttu-id="4ab56-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ab56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ab56-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ab56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ab56-106">Recupere as propriedades e os relacionamentos de um objeto [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="4ab56-106">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ab56-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ab56-107">Permissions</span></span>
<span data-ttu-id="4ab56-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab56-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ab56-110">Permission type</span></span>      | <span data-ttu-id="4ab56-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ab56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ab56-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ab56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ab56-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab56-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ab56-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ab56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab56-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ab56-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4ab56-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ab56-116">Application</span></span> | <span data-ttu-id="4ab56-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab56-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ab56-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ab56-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ab56-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ab56-119">Optional query parameters</span></span>
<span data-ttu-id="4ab56-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab56-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4ab56-p103">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `name` e `self`. Os valores `expand` válidos para o grupo de seção são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="4ab56-p103">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ab56-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab56-123">Request headers</span></span>
| <span data-ttu-id="4ab56-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4ab56-124">Name</span></span>       | <span data-ttu-id="4ab56-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ab56-125">Type</span></span> | <span data-ttu-id="4ab56-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ab56-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4ab56-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ab56-127">Authorization</span></span>  | <span data-ttu-id="4ab56-128">string</span><span class="sxs-lookup"><span data-stu-id="4ab56-128">string</span></span>  | <span data-ttu-id="4ab56-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ab56-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ab56-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ab56-131">Accept</span></span> | <span data-ttu-id="4ab56-132">string</span><span class="sxs-lookup"><span data-stu-id="4ab56-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4ab56-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab56-133">Request body</span></span>
<span data-ttu-id="4ab56-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ab56-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab56-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab56-135">Response</span></span>

<span data-ttu-id="4ab56-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [sectionGroup](../resources/sectiongroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ab56-136">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ab56-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ab56-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ab56-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ab56-138">Request</span></span>
<span data-ttu-id="4ab56-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ab56-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="4ab56-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ab56-140">Response</span></span>
<span data-ttu-id="4ab56-p105">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ab56-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->