---
title: Obter diretiva
description: Recupere as propriedades de uma política.
localization_priority: Normal
ms.openlocfilehash: 9b3e23639bdeea673ccbe56bbce0c74443a99480
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870592"
---
# <a name="get-policy"></a><span data-ttu-id="e6cf3-103">Obter diretiva</span><span class="sxs-lookup"><span data-stu-id="e6cf3-103">Get Policy</span></span>

> <span data-ttu-id="e6cf3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6cf3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6cf3-106">Recupere as propriedades de uma [diretiva](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="e6cf3-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6cf3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e6cf3-107">Permissions</span></span>
<span data-ttu-id="e6cf3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6cf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6cf3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6cf3-110">Permission type</span></span>      | <span data-ttu-id="e6cf3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6cf3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6cf3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6cf3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6cf3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6cf3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6cf3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6cf3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6cf3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-115">Not supported.</span></span>    |
|<span data-ttu-id="e6cf3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6cf3-116">Application</span></span> | <span data-ttu-id="e6cf3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6cf3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6cf3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e6cf3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cf3-119">Request headers</span></span>
| <span data-ttu-id="e6cf3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6cf3-120">Name</span></span>       | <span data-ttu-id="e6cf3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6cf3-121">Type</span></span> | <span data-ttu-id="e6cf3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cf3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6cf3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6cf3-123">Authorization</span></span>  | <span data-ttu-id="e6cf3-124">string</span><span class="sxs-lookup"><span data-stu-id="e6cf3-124">string</span></span>  | <span data-ttu-id="e6cf3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6cf3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cf3-127">Request body</span></span>
<span data-ttu-id="e6cf3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6cf3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cf3-129">Response</span></span>

<span data-ttu-id="e6cf3-130">Se tiver êxito, este método retornará `200 OK` código de resposta e um objeto de [política](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="e6cf3-131">Se unsucccessful …</span><span class="sxs-lookup"><span data-stu-id="e6cf3-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="e6cf3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6cf3-132">Example</span></span>
<span data-ttu-id="e6cf3-133">O exemplo a seguir recupera uma diretiva específica.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="e6cf3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cf3-134">Request</span></span>
<span data-ttu-id="e6cf3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="e6cf3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cf3-136">Response</span></span>
<span data-ttu-id="e6cf3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6cf3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
