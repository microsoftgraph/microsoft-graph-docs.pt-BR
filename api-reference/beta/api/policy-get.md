---
title: Obter política
description: Recupere as propriedades de uma política.
localization_priority: Normal
ms.openlocfilehash: 853809ad26910b73bcf6c957e4c55e60f04dea49
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332208"
---
# <a name="get-policy"></a><span data-ttu-id="55f20-103">Obter política</span><span class="sxs-lookup"><span data-stu-id="55f20-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55f20-104">Recupere as propriedades de uma [política](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="55f20-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55f20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="55f20-105">Permissions</span></span>
<span data-ttu-id="55f20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55f20-108">Permission type</span></span>      | <span data-ttu-id="55f20-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55f20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55f20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55f20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55f20-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55f20-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55f20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55f20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55f20-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55f20-113">Not supported.</span></span>    |
|<span data-ttu-id="55f20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55f20-114">Application</span></span> | <span data-ttu-id="55f20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55f20-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55f20-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55f20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="55f20-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55f20-117">Request headers</span></span>
| <span data-ttu-id="55f20-118">Nome</span><span class="sxs-lookup"><span data-stu-id="55f20-118">Name</span></span>       | <span data-ttu-id="55f20-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="55f20-119">Type</span></span> | <span data-ttu-id="55f20-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55f20-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55f20-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="55f20-121">Authorization</span></span>  | <span data-ttu-id="55f20-122">string</span><span class="sxs-lookup"><span data-stu-id="55f20-122">string</span></span>  | <span data-ttu-id="55f20-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55f20-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55f20-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55f20-125">Request body</span></span>
<span data-ttu-id="55f20-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55f20-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55f20-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f20-127">Response</span></span>

<span data-ttu-id="55f20-128">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55f20-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="55f20-129">Se unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="55f20-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="55f20-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55f20-130">Example</span></span>
<span data-ttu-id="55f20-131">O exemplo a seguir recupera uma política específica.</span><span class="sxs-lookup"><span data-stu-id="55f20-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="55f20-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55f20-132">Request</span></span>
<span data-ttu-id="55f20-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55f20-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="55f20-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f20-134">Response</span></span>
<span data-ttu-id="55f20-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55f20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
