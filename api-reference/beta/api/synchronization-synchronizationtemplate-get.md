---
title: Obter synchronizationtemplate
description: Recupere um modelo de sincronização por seu identificador.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ef1c33422b36e8fd88fcc6646506905e2a091e1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991097"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="852fb-103">Obter synchronizationtemplate</span><span class="sxs-lookup"><span data-stu-id="852fb-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="852fb-104">Recupere um modelo de sincronização por seu identificador.</span><span class="sxs-lookup"><span data-stu-id="852fb-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="852fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="852fb-105">Permissions</span></span>
<span data-ttu-id="852fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="852fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="852fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="852fb-108">Permission type</span></span>                        | <span data-ttu-id="852fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="852fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="852fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="852fb-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="852fb-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="852fb-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="852fb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="852fb-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="852fb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="852fb-113">Not supported.</span></span>|
|<span data-ttu-id="852fb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="852fb-114">Application</span></span>                            |<span data-ttu-id="852fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="852fb-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="852fb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="852fb-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="852fb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="852fb-117">Request headers</span></span>

| <span data-ttu-id="852fb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="852fb-118">Name</span></span>           | <span data-ttu-id="852fb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="852fb-119">Type</span></span>    | <span data-ttu-id="852fb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="852fb-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="852fb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="852fb-121">Authorization</span></span>  | <span data-ttu-id="852fb-122">string</span><span class="sxs-lookup"><span data-stu-id="852fb-122">string</span></span>  | <span data-ttu-id="852fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="852fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="852fb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="852fb-125">Request body</span></span>

<span data-ttu-id="852fb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="852fb-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="852fb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="852fb-127">Response</span></span>

<span data-ttu-id="852fb-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="852fb-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="852fb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="852fb-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="852fb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="852fb-130">Request</span></span>
<span data-ttu-id="852fb-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="852fb-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="852fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="852fb-132">Response</span></span>
<span data-ttu-id="852fb-133">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="852fb-133">The following is an example of a response.</span></span>
><span data-ttu-id="852fb-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="852fb-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="852fb-135">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="852fb-135">All the properties will be returned in an actual call.</span></span>

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
