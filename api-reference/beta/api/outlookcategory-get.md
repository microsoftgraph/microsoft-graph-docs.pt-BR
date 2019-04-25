---
title: Obter categoria do Outlook
description: Obtenha as propriedades e as relações do objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7529568b26c56258e63a8c1080c019aaf0f57e59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539707"
---
# <a name="get-outlook-category"></a><span data-ttu-id="d74aa-103">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="d74aa-103">Get Outlook category</span></span>


<span data-ttu-id="d74aa-104">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="d74aa-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d74aa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d74aa-105">Permissions</span></span>
<span data-ttu-id="d74aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d74aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74aa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d74aa-108">Permission type</span></span>      | <span data-ttu-id="d74aa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d74aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d74aa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d74aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d74aa-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d74aa-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d74aa-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d74aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d74aa-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d74aa-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="d74aa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d74aa-114">Application</span></span> | <span data-ttu-id="d74aa-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="d74aa-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d74aa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d74aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d74aa-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d74aa-117">Optional query parameters</span></span>
<span data-ttu-id="d74aa-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d74aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d74aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d74aa-119">Request headers</span></span>
| <span data-ttu-id="d74aa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d74aa-120">Name</span></span>      |<span data-ttu-id="d74aa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74aa-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d74aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d74aa-122">Authorization</span></span>  | <span data-ttu-id="d74aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d74aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d74aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d74aa-125">Request body</span></span>
<span data-ttu-id="d74aa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d74aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d74aa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d74aa-127">Response</span></span>

<span data-ttu-id="d74aa-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d74aa-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d74aa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d74aa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d74aa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d74aa-130">Request</span></span>
<span data-ttu-id="d74aa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d74aa-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="d74aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d74aa-132">Response</span></span>
<span data-ttu-id="d74aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d74aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
