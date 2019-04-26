---
title: Listar políticas
description: Recupere todos os objetos de política no diretório.
localization_priority: Normal
ms.openlocfilehash: 7f4b70391b68a47073866248c31395df4ebaaf45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337373"
---
# <a name="list-policies"></a><span data-ttu-id="5c37a-103">Listar políticas</span><span class="sxs-lookup"><span data-stu-id="5c37a-103">List Policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c37a-104">Recupere todos os objetos de [política](../resources/policy.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="5c37a-104">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c37a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c37a-105">Permissions</span></span>
<span data-ttu-id="5c37a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c37a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c37a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c37a-108">Permission type</span></span>      | <span data-ttu-id="5c37a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c37a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c37a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c37a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c37a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c37a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c37a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c37a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c37a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c37a-113">Not supported.</span></span>    |
|<span data-ttu-id="5c37a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c37a-114">Application</span></span> | <span data-ttu-id="5c37a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c37a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c37a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c37a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="5c37a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c37a-117">Request headers</span></span>
| <span data-ttu-id="5c37a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5c37a-118">Name</span></span>       | <span data-ttu-id="5c37a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c37a-119">Type</span></span> | <span data-ttu-id="5c37a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c37a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c37a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c37a-121">Authorization</span></span>  | <span data-ttu-id="5c37a-122">string</span><span class="sxs-lookup"><span data-stu-id="5c37a-122">string</span></span>  | <span data-ttu-id="5c37a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c37a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c37a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c37a-125">Request body</span></span>
<span data-ttu-id="5c37a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c37a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c37a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c37a-127">Response</span></span>

<span data-ttu-id="5c37a-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e os objetos [Policy](../resources/policy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c37a-128">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="5c37a-129">Se não tiver êxito...</span><span class="sxs-lookup"><span data-stu-id="5c37a-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="5c37a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c37a-130">Example</span></span>
<span data-ttu-id="5c37a-131">O exemplo a seguir recupera todas as políticas.</span><span class="sxs-lookup"><span data-stu-id="5c37a-131">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="5c37a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c37a-132">Request</span></span>
<span data-ttu-id="5c37a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c37a-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="5c37a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c37a-134">Response</span></span>
<span data-ttu-id="5c37a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c37a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
