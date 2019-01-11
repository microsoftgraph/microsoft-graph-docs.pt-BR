---
title: 'privilegedRoleAssignment: meu'
description: Obtenha as atribuições de função privilegiado do solicitador.
localization_priority: Normal
ms.openlocfilehash: fca950413d2f0a50b6ea9e09b859d2ecf926261b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840254"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="9dce9-103">privilegedRoleAssignment: meu</span><span class="sxs-lookup"><span data-stu-id="9dce9-103">privilegedRoleAssignment: my</span></span>

> <span data-ttu-id="9dce9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9dce9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dce9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9dce9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9dce9-106">Obtenha as atribuições de função privilegiado do solicitador.</span><span class="sxs-lookup"><span data-stu-id="9dce9-106">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dce9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9dce9-107">Permissions</span></span>
<span data-ttu-id="9dce9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dce9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dce9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dce9-110">Permission type</span></span>      | <span data-ttu-id="9dce9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9dce9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dce9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dce9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9dce9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9dce9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9dce9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dce9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dce9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dce9-115">Not supported.</span></span>    |
|<span data-ttu-id="9dce9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dce9-116">Application</span></span> | <span data-ttu-id="9dce9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dce9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dce9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dce9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="9dce9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dce9-119">Request headers</span></span>
| <span data-ttu-id="9dce9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9dce9-120">Name</span></span>       | <span data-ttu-id="9dce9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dce9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dce9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dce9-122">Authorization</span></span>  | <span data-ttu-id="9dce9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dce9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dce9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dce9-125">Request body</span></span>
<span data-ttu-id="9dce9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9dce9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dce9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dce9-127">Response</span></span>

<span data-ttu-id="9dce9-128">Se tiver êxito, este método retornará `200 OK` objeto de coleção [privilegedRoleAssignment](../resources/privilegedroleassignment.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dce9-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dce9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9dce9-129">Example</span></span>
<span data-ttu-id="9dce9-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9dce9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9dce9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dce9-131">Request</span></span>
<span data-ttu-id="9dce9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dce9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="9dce9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dce9-133">Response</span></span>
<span data-ttu-id="9dce9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dce9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
