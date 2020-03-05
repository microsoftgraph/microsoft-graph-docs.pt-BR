---
title: Listar políticas
description: Obtenha todos os objetos de política no diretório.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 0f3119d79ed7c9dfa37453aa90bf0b95eecb901b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455505"
---
# <a name="list-policies"></a><span data-ttu-id="6d67e-103">Listar políticas</span><span class="sxs-lookup"><span data-stu-id="6d67e-103">List Policies</span></span>

<span data-ttu-id="6d67e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d67e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d67e-105">Obtenha todos os objetos de [política](../resources/policy.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="6d67e-105">Get all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d67e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d67e-106">Permissions</span></span>
<span data-ttu-id="6d67e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d67e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d67e-109">Permission type</span></span>      | <span data-ttu-id="6d67e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d67e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d67e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d67e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6d67e-112">Policy. Read. All, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6d67e-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d67e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d67e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d67e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d67e-114">Not supported.</span></span>    |
|<span data-ttu-id="6d67e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d67e-115">Application</span></span> | <span data-ttu-id="6d67e-116">Policy. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="6d67e-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d67e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d67e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="6d67e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d67e-118">Request headers</span></span>
| <span data-ttu-id="6d67e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6d67e-119">Name</span></span>       | <span data-ttu-id="6d67e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d67e-120">Type</span></span> | <span data-ttu-id="6d67e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d67e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d67e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d67e-122">Authorization</span></span>  | <span data-ttu-id="6d67e-123">string</span><span class="sxs-lookup"><span data-stu-id="6d67e-123">string</span></span>  | <span data-ttu-id="6d67e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d67e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d67e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d67e-126">Request body</span></span>
<span data-ttu-id="6d67e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d67e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d67e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d67e-128">Response</span></span>

<span data-ttu-id="6d67e-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d67e-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="6d67e-130">Se não tiver êxito...</span><span class="sxs-lookup"><span data-stu-id="6d67e-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="6d67e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d67e-131">Example</span></span>
<span data-ttu-id="6d67e-132">O exemplo a seguir recupera todas as políticas.</span><span class="sxs-lookup"><span data-stu-id="6d67e-132">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="6d67e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d67e-133">Request</span></span>
<span data-ttu-id="6d67e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d67e-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="6d67e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d67e-135">Response</span></span>
<span data-ttu-id="6d67e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d67e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
