---
title: Obter identityUserFlowAttribute
description: Recupere as propriedades e os relacionamentos de um objeto identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8d1d60a318ebe3962af0077b367b334d37420a4
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742342"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="9be3e-103">Obter identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="9be3e-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="9be3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be3e-105">Recupere as propriedades e os relacionamentos de um objeto [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="9be3e-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9be3e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9be3e-106">Permissions</span></span>

<span data-ttu-id="9be3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9be3e-109">Permission type</span></span>      | <span data-ttu-id="9be3e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9be3e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be3e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9be3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9be3e-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9be3e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9be3e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9be3e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9be3e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9be3e-114">Not supported.</span></span>|
|<span data-ttu-id="9be3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9be3e-115">Application</span></span>|<span data-ttu-id="9be3e-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9be3e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9be3e-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9be3e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9be3e-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9be3e-118">Global administrator</span></span>
* <span data-ttu-id="9be3e-119">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="9be3e-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9be3e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9be3e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9be3e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9be3e-121">Request headers</span></span>

|<span data-ttu-id="9be3e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9be3e-122">Name</span></span>|<span data-ttu-id="9be3e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be3e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9be3e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9be3e-124">Authorization</span></span>|<span data-ttu-id="9be3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9be3e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9be3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9be3e-127">Request body</span></span>

<span data-ttu-id="9be3e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9be3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9be3e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be3e-129">Response</span></span>

<span data-ttu-id="9be3e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityUserFlowAttribute](../resources/identityuserflowattribute.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9be3e-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be3e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9be3e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9be3e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9be3e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="9be3e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9be3e-133">Response</span></span>

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
