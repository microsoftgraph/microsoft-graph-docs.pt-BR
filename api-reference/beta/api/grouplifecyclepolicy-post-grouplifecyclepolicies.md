---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b7e523f28c92547d2e2b1e11377418a517351b31
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879216"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="78e9b-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="78e9b-103">Create groupLifecyclePolicy</span></span>

> <span data-ttu-id="78e9b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78e9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78e9b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78e9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78e9b-106">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="78e9b-106">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78e9b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78e9b-107">Permissions</span></span>

<span data-ttu-id="78e9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78e9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="78e9b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78e9b-110">Permission type</span></span>      | <span data-ttu-id="78e9b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78e9b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78e9b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78e9b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78e9b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e9b-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="78e9b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78e9b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78e9b-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="78e9b-115">Not supported</span></span> |
|<span data-ttu-id="78e9b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78e9b-116">Application</span></span> |  <span data-ttu-id="78e9b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e9b-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78e9b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78e9b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="78e9b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78e9b-119">Request headers</span></span>

| <span data-ttu-id="78e9b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="78e9b-120">Name</span></span> | <span data-ttu-id="78e9b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="78e9b-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="78e9b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78e9b-122">Authorization</span></span> | <span data-ttu-id="78e9b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78e9b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78e9b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78e9b-125">Content-Type</span></span>  | <span data-ttu-id="78e9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e9b-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="78e9b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78e9b-127">Request body</span></span>
<span data-ttu-id="78e9b-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="78e9b-128">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78e9b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e9b-129">Response</span></span>

<span data-ttu-id="78e9b-130">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78e9b-130">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e9b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78e9b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="78e9b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78e9b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="78e9b-133">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="78e9b-133">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="78e9b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="78e9b-134">Response</span></span>

<span data-ttu-id="78e9b-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78e9b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
