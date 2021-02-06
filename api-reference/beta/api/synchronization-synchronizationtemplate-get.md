---
title: Obter synchronizationTemplate
description: Recupere um modelo de sincronização por seu identificador.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8887896e734a2fd1d81d9a3e9c14e36125e78a9c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136336"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="6f614-103">Obter synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="6f614-103">Get synchronizationTemplate</span></span>

<span data-ttu-id="6f614-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f614-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f614-105">Recupere um modelo de sincronização por seu identificador.</span><span class="sxs-lookup"><span data-stu-id="6f614-105">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f614-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f614-106">Permissions</span></span>
<span data-ttu-id="6f614-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f614-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f614-109">Permission type</span></span>                        | <span data-ttu-id="6f614-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f614-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f614-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f614-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="6f614-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f614-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6f614-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f614-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6f614-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f614-114">Not supported.</span></span>|
|<span data-ttu-id="6f614-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f614-115">Application</span></span>                            |<span data-ttu-id="6f614-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f614-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="6f614-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f614-117">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="6f614-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f614-118">Request headers</span></span>

| <span data-ttu-id="6f614-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6f614-119">Name</span></span>           | <span data-ttu-id="6f614-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f614-120">Type</span></span>    | <span data-ttu-id="6f614-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f614-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6f614-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f614-122">Authorization</span></span>  | <span data-ttu-id="6f614-123">string</span><span class="sxs-lookup"><span data-stu-id="6f614-123">string</span></span>  | <span data-ttu-id="6f614-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f614-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f614-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f614-126">Request body</span></span>

<span data-ttu-id="6f614-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f614-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6f614-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f614-128">Response</span></span>

<span data-ttu-id="6f614-129">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f614-129">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="6f614-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f614-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f614-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f614-131">Request</span></span>
<span data-ttu-id="6f614-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f614-132">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="6f614-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f614-133">Response</span></span>
<span data-ttu-id="6f614-134">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6f614-134">The following is an example of a response.</span></span>
><span data-ttu-id="6f614-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f614-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6f614-136">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f614-136">All the properties will be returned in an actual call.</span></span>

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


