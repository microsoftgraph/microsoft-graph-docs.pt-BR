---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: dkershaw10
ms.openlocfilehash: ef239385766b33c4a03576200c6c9abf3938c25a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312520"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="a6120-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a6120-103">Get groupLifecyclePolicy</span></span>

> <span data-ttu-id="a6120-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6120-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6120-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6120-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6120-106">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a6120-106">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6120-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6120-107">Permissions</span></span>

<span data-ttu-id="a6120-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6120-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a6120-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6120-110">Permission type</span></span>      | <span data-ttu-id="a6120-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6120-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6120-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6120-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6120-113">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6120-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a6120-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6120-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6120-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a6120-115">Not supported</span></span> |
|<span data-ttu-id="a6120-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6120-116">Application</span></span> | <span data-ttu-id="a6120-117">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6120-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6120-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6120-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6120-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6120-119">Optional query parameters</span></span>
<span data-ttu-id="a6120-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6120-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6120-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6120-121">Request headers</span></span>
| <span data-ttu-id="a6120-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a6120-122">Name</span></span> | <span data-ttu-id="a6120-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6120-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a6120-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6120-124">Authorization</span></span> | <span data-ttu-id="a6120-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6120-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6120-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6120-127">Request body</span></span>
<span data-ttu-id="a6120-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6120-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a6120-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6120-129">Response</span></span>
<span data-ttu-id="a6120-130">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6120-130">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6120-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6120-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6120-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6120-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="a6120-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6120-133">Response</span></span>

<span data-ttu-id="a6120-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6120-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->