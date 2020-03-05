---
title: Obter synchronizationtemplate
description: Recupere um modelo de sincronização por seu identificador.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f75f25eb44693ce4158bdbf1e8de1047fecadef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452880"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="3e45f-103">Obter synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="3e45f-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="3e45f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e45f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e45f-105">Recupere um modelo de sincronização por seu identificador.</span><span class="sxs-lookup"><span data-stu-id="3e45f-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e45f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e45f-106">Permissions</span></span>
<span data-ttu-id="3e45f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e45f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e45f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e45f-109">Permission type</span></span>                        | <span data-ttu-id="3e45f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e45f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e45f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e45f-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="3e45f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e45f-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3e45f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e45f-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3e45f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e45f-114">Not supported.</span></span>|
|<span data-ttu-id="3e45f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e45f-115">Application</span></span>                            |<span data-ttu-id="3e45f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e45f-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="3e45f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e45f-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="3e45f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e45f-118">Request headers</span></span>

| <span data-ttu-id="3e45f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3e45f-119">Name</span></span>           | <span data-ttu-id="3e45f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e45f-120">Type</span></span>    | <span data-ttu-id="3e45f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e45f-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3e45f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e45f-122">Authorization</span></span>  | <span data-ttu-id="3e45f-123">string</span><span class="sxs-lookup"><span data-stu-id="3e45f-123">string</span></span>  | <span data-ttu-id="3e45f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e45f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e45f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e45f-126">Request body</span></span>

<span data-ttu-id="3e45f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e45f-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="3e45f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e45f-128">Response</span></span>

<span data-ttu-id="3e45f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e45f-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="3e45f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e45f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3e45f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e45f-131">Request</span></span>
<span data-ttu-id="3e45f-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e45f-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="3e45f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e45f-133">Response</span></span>
<span data-ttu-id="3e45f-134">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3e45f-134">The following is an example of a response.</span></span>
><span data-ttu-id="3e45f-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e45f-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e45f-136">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e45f-136">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
