---
title: Obter diretiva
description: Recupere as propriedades de uma política.
ms.openlocfilehash: a6827813193d134f54c3274e2b035e241bb99dc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034418"
---
# <a name="get-policy"></a><span data-ttu-id="749eb-103">Obter diretiva</span><span class="sxs-lookup"><span data-stu-id="749eb-103">Get Policy</span></span>

> <span data-ttu-id="749eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="749eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="749eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="749eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="749eb-106">Recupere as propriedades de uma [diretiva](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="749eb-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="749eb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="749eb-107">Permissions</span></span>
<span data-ttu-id="749eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="749eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="749eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="749eb-110">Permission type</span></span>      | <span data-ttu-id="749eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="749eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="749eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="749eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="749eb-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="749eb-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="749eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="749eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="749eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="749eb-115">Not supported.</span></span>    |
|<span data-ttu-id="749eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="749eb-116">Application</span></span> | <span data-ttu-id="749eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="749eb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="749eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="749eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="749eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="749eb-119">Request headers</span></span>
| <span data-ttu-id="749eb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="749eb-120">Name</span></span>       | <span data-ttu-id="749eb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="749eb-121">Type</span></span> | <span data-ttu-id="749eb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="749eb-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="749eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="749eb-123">Authorization</span></span>  | <span data-ttu-id="749eb-124">string</span><span class="sxs-lookup"><span data-stu-id="749eb-124">string</span></span>  | <span data-ttu-id="749eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="749eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="749eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="749eb-127">Request body</span></span>
<span data-ttu-id="749eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="749eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="749eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="749eb-129">Response</span></span>

<span data-ttu-id="749eb-130">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto de [política](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="749eb-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="749eb-131">Se unsucccessful …</span><span class="sxs-lookup"><span data-stu-id="749eb-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="749eb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="749eb-132">Example</span></span>
<span data-ttu-id="749eb-133">O exemplo a seguir recupera uma diretiva específica.</span><span class="sxs-lookup"><span data-stu-id="749eb-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="749eb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="749eb-134">Request</span></span>
<span data-ttu-id="749eb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="749eb-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="749eb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="749eb-136">Response</span></span>
<span data-ttu-id="749eb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="749eb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
