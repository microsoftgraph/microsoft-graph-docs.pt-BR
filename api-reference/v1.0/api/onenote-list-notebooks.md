---
title: Listar blocos de anotações
description: Recuperar uma lista de objetos do bloco de anotações.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b66b059d92b1177a6c2b5df9a9d978eb87dec53e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562143"
---
# <a name="list-notebooks"></a><span data-ttu-id="93ede-103">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="93ede-103">List notebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93ede-104">Recupere uma lista de objetos [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="93ede-104">Retrieve a list of [profilePhoto](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="93ede-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="93ede-105">Permissions</span></span>
<span data-ttu-id="93ede-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ede-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93ede-108">Permission type</span></span>      | <span data-ttu-id="93ede-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93ede-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93ede-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93ede-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93ede-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ede-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>    |
|<span data-ttu-id="93ede-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93ede-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93ede-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93ede-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="93ede-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93ede-114">Application</span></span> | <span data-ttu-id="93ede-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ede-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93ede-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93ede-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="93ede-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93ede-117">Optional query parameters</span></span>
<span data-ttu-id="93ede-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="93ede-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="93ede-119">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="93ede-119">The default sort order for notebooks is `name asc`.</span></span> 

<span data-ttu-id="93ede-120">Os valores `expand` válidos para os blocos de anotações são `sections` e `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="93ede-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93ede-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93ede-121">Request headers</span></span>
| <span data-ttu-id="93ede-122">Nome</span><span class="sxs-lookup"><span data-stu-id="93ede-122">Name</span></span>       | <span data-ttu-id="93ede-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="93ede-123">Type</span></span> | <span data-ttu-id="93ede-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="93ede-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="93ede-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="93ede-125">Authorization</span></span>  | <span data-ttu-id="93ede-126">string</span><span class="sxs-lookup"><span data-stu-id="93ede-126">string</span></span>  | <span data-ttu-id="93ede-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93ede-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93ede-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93ede-129">Accept</span></span> | <span data-ttu-id="93ede-130">string</span><span class="sxs-lookup"><span data-stu-id="93ede-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="93ede-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93ede-131">Request body</span></span>
<span data-ttu-id="93ede-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93ede-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93ede-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ede-133">Response</span></span>

<span data-ttu-id="93ede-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [notebook](../resources/notebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93ede-134">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="93ede-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93ede-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93ede-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93ede-136">Request</span></span>
<span data-ttu-id="93ede-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93ede-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="93ede-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ede-138">Response</span></span>
<span data-ttu-id="93ede-p103">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93ede-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
