---
title: Lista de políticas
description: Recupere todos os objetos de política no diretório.
localization_priority: Normal
ms.openlocfilehash: ea97146b646068515ab6fdc7fab4b3cefb16031e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836052"
---
# <a name="list-policies"></a><span data-ttu-id="7c5c9-103">Lista de políticas</span><span class="sxs-lookup"><span data-stu-id="7c5c9-103">List Policies</span></span>

> <span data-ttu-id="7c5c9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c5c9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c5c9-106">Recupere todos os objetos de [política](../resources/policy.md) no diretório.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c5c9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7c5c9-107">Permissions</span></span>
<span data-ttu-id="7c5c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c5c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c5c9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c5c9-110">Permission type</span></span>      | <span data-ttu-id="7c5c9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c5c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c5c9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c5c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c5c9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c5c9-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c5c9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c5c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c5c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-115">Not supported.</span></span>    |
|<span data-ttu-id="7c5c9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c5c9-116">Application</span></span> | <span data-ttu-id="7c5c9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c5c9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c5c9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="7c5c9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5c9-119">Request headers</span></span>
| <span data-ttu-id="7c5c9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7c5c9-120">Name</span></span>       | <span data-ttu-id="7c5c9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c5c9-121">Type</span></span> | <span data-ttu-id="7c5c9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c5c9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c5c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c5c9-123">Authorization</span></span>  | <span data-ttu-id="7c5c9-124">string</span><span class="sxs-lookup"><span data-stu-id="7c5c9-124">string</span></span>  | <span data-ttu-id="7c5c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c5c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5c9-127">Request body</span></span>
<span data-ttu-id="7c5c9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c5c9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c5c9-129">Response</span></span>

<span data-ttu-id="7c5c9-130">Se tiver êxito, este método retornará `200 OK` objetos de código e a [diretiva](../resources/policy.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="7c5c9-131">Se não houver êxito …</span><span class="sxs-lookup"><span data-stu-id="7c5c9-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="7c5c9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c5c9-132">Example</span></span>
<span data-ttu-id="7c5c9-133">O exemplo a seguir recupera todas as diretivas.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="7c5c9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c5c9-134">Request</span></span>
<span data-ttu-id="7c5c9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="7c5c9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c5c9-136">Response</span></span>
<span data-ttu-id="7c5c9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c5c9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
