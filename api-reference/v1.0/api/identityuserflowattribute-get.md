---
title: Obter identityUserFlowAttribute
description: Recupere as propriedades e as relações de um objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2396e09e10acdb82c914f888a2ebdada523da78a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882383"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="8968d-103">Obter identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="8968d-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="8968d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8968d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8968d-105">Recupere as propriedades e as relações de [um objeto identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="8968d-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8968d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8968d-106">Permissions</span></span>

<span data-ttu-id="8968d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8968d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8968d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8968d-109">Permission type</span></span>      | <span data-ttu-id="8968d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8968d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8968d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8968d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8968d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8968d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8968d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8968d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8968d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8968d-114">Not supported.</span></span>|
|<span data-ttu-id="8968d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8968d-115">Application</span></span>|<span data-ttu-id="8968d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8968d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8968d-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="8968d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8968d-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8968d-118">Global administrator</span></span>
* <span data-ttu-id="8968d-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="8968d-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8968d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8968d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8968d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8968d-121">Request headers</span></span>

|<span data-ttu-id="8968d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8968d-122">Name</span></span>|<span data-ttu-id="8968d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8968d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8968d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8968d-124">Authorization</span></span>|<span data-ttu-id="8968d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8968d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8968d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8968d-127">Request body</span></span>

<span data-ttu-id="8968d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8968d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8968d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8968d-129">Response</span></span>

<span data-ttu-id="8968d-130">Se tiver êxito, este método retornará um código de resposta e uma representação JSON da `200 OK` [identidadeUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8968d-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8968d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8968d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8968d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8968d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="8968d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8968d-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
