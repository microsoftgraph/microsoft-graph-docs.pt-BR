---
title: Criar responsáveis
description: Criar um novo objeto de responsáveis.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7142d00f7fdee7643e5c6c2b755c1c88a1e9f9dc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597520"
---
# <a name="create-custodian"></a><span data-ttu-id="caef4-103">Criar responsáveis</span><span class="sxs-lookup"><span data-stu-id="caef4-103">Create custodian</span></span>

<span data-ttu-id="caef4-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="caef4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caef4-105">Criar um novo objeto de [responsáveis](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="caef4-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="caef4-106">Depois que o objeto responsáveis for criado, você precisará criar o [usuário](../resources/usersource.md) do responsáveis para fazer referência à caixa de correio e ao site do onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="caef4-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="caef4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="caef4-107">Permissions</span></span>

<span data-ttu-id="caef4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caef4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caef4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caef4-110">Permission type</span></span>|<span data-ttu-id="caef4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="caef4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caef4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caef4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="caef4-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="caef4-113">User.Read</span></span>|
|<span data-ttu-id="caef4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caef4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caef4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caef4-115">Not supported.</span></span>|
|<span data-ttu-id="caef4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caef4-116">Application</span></span>|<span data-ttu-id="caef4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caef4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caef4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caef4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="caef4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caef4-119">Request headers</span></span>

|<span data-ttu-id="caef4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="caef4-120">Name</span></span>|<span data-ttu-id="caef4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="caef4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="caef4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="caef4-122">Authorization</span></span>|<span data-ttu-id="caef4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caef4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="caef4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="caef4-125">Content-Type</span></span>|<span data-ttu-id="caef4-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caef4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="caef4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caef4-128">Request body</span></span>

<span data-ttu-id="caef4-129">No corpo da solicitação, forneça uma representação JSON do objeto [responsáveis](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="caef4-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="caef4-130">A tabela a seguir mostra as propriedades que são necessárias ao criar os [responsáveis](../resources/custodian.md).</span><span class="sxs-lookup"><span data-stu-id="caef4-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="caef4-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caef4-131">Property</span></span>|<span data-ttu-id="caef4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="caef4-132">Type</span></span>|<span data-ttu-id="caef4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="caef4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caef4-134">email</span><span class="sxs-lookup"><span data-stu-id="caef4-134">email</span></span>|<span data-ttu-id="caef4-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="caef4-135">String</span></span>|<span data-ttu-id="caef4-136">Endereço SMTP principal do responsáveis.</span><span class="sxs-lookup"><span data-stu-id="caef4-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="caef4-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caef4-137">Required.</span></span>|
|<span data-ttu-id="caef4-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="caef4-138">applyHoldToSources</span></span>|<span data-ttu-id="caef4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="caef4-139">Boolean</span></span>|<span data-ttu-id="caef4-140">Indica se uma retenção é aplicada às fontes dos responsáveis (como caixas de correio, sites ou equipes).</span><span class="sxs-lookup"><span data-stu-id="caef4-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="caef4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="caef4-141">Response</span></span>

<span data-ttu-id="caef4-142">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [responsáveis](../resources/custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caef4-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="caef4-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="caef4-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="caef4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caef4-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```

### <a name="response"></a><span data-ttu-id="caef4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="caef4-145">Response</span></span>

<span data-ttu-id="caef4-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="caef4-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
