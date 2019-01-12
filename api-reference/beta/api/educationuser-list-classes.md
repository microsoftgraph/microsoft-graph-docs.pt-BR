---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: fe950190ce3bd56b5f236f42a840d3d0b9f5d130
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960921"
---
# <a name="list-classes"></a><span data-ttu-id="df055-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="df055-104">List classes</span></span>

> <span data-ttu-id="df055-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df055-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df055-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df055-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df055-107">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="df055-107">Retrieve a list of class objects.</span></span> <span data-ttu-id="df055-108">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="df055-108">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="df055-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="df055-109">Permissions</span></span>
<span data-ttu-id="df055-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df055-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df055-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df055-112">Permission type</span></span>      | <span data-ttu-id="df055-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df055-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df055-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df055-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="df055-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="df055-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="df055-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df055-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df055-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df055-117">Not supported.</span></span>  |
|<span data-ttu-id="df055-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df055-118">Application</span></span> | <span data-ttu-id="df055-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df055-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df055-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df055-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="df055-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="df055-121">Optional query parameters</span></span>
<span data-ttu-id="df055-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="df055-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df055-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df055-123">Request headers</span></span>
| <span data-ttu-id="df055-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df055-124">Header</span></span>       | <span data-ttu-id="df055-125">Valor</span><span class="sxs-lookup"><span data-stu-id="df055-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df055-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="df055-126">Authorization</span></span>  | <span data-ttu-id="df055-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df055-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df055-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df055-129">Request body</span></span>
<span data-ttu-id="df055-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df055-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="df055-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="df055-131">Response</span></span>
<span data-ttu-id="df055-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df055-132">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df055-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df055-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df055-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df055-134">Request</span></span>
<span data-ttu-id="df055-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df055-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="df055-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="df055-136">Response</span></span>
<span data-ttu-id="df055-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df055-137">The following is an example of the response.</span></span> 

><span data-ttu-id="df055-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df055-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
