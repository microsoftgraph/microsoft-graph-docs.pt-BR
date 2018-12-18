---
title: Obtenha uma configuração de grupo
description: Recupere as propriedades de um determinado objeto de configuração de grupo.
author: dkershaw10
ms.openlocfilehash: 567fc7a38f95f295ca6d896b1aed6c456abbab4c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339064"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="b5b55-103">Obtenha uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="b5b55-103">Get a group setting</span></span>

<span data-ttu-id="b5b55-104">Recupere as propriedades de um determinado objeto de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="b5b55-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5b55-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5b55-105">Permissions</span></span>

<span data-ttu-id="b5b55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5b55-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5b55-108">Permission type</span></span>      | <span data-ttu-id="b5b55-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5b55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5b55-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5b55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5b55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5b55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5b55-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5b55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5b55-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5b55-113">Not supported.</span></span>    |
|<span data-ttu-id="b5b55-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5b55-114">Application</span></span> | <span data-ttu-id="b5b55-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b55-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5b55-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5b55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b5b55-117">Obter uma configuração de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="b5b55-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5b55-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5b55-118">Optional query parameters</span></span>
<span data-ttu-id="b5b55-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5b55-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="b5b55-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="b5b55-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5b55-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b55-121">Request headers</span></span>
| <span data-ttu-id="b5b55-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b5b55-122">Name</span></span> | <span data-ttu-id="b5b55-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5b55-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b5b55-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5b55-124">Authorization</span></span> | <span data-ttu-id="b5b55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5b55-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5b55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b55-127">Request body</span></span>

<span data-ttu-id="b5b55-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5b55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5b55-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5b55-129">Response</span></span>

<span data-ttu-id="b5b55-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5b55-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b55-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5b55-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5b55-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b55-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="b5b55-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5b55-133">Response</span></span>

<span data-ttu-id="b5b55-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5b55-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->