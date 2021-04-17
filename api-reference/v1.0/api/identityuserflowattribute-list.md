---
title: Listar identityUserFlowAttributes
description: Recupere uma lista de objetos identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4d0a596f8710d319f5c57e651e1fa59a997e88b2
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882384"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="fdb8c-103">Listar identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="fdb8c-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="fdb8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb8c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdb8c-105">Recupere uma lista de [objetos identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="fdb8c-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdb8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdb8c-106">Permissions</span></span>

<span data-ttu-id="fdb8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdb8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdb8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdb8c-109">Permission type</span></span>      | <span data-ttu-id="fdb8c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdb8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdb8c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdb8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdb8c-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb8c-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="fdb8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdb8c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fdb8c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-114">Not supported.</span></span>|
|<span data-ttu-id="fdb8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdb8c-115">Application</span></span>|<span data-ttu-id="fdb8c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb8c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fdb8c-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fdb8c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fdb8c-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fdb8c-118">Global administrator</span></span>
* <span data-ttu-id="fdb8c-119">Administrador de Atributo de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fdb8c-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fdb8c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb8c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="fdb8c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb8c-121">Request headers</span></span>

|<span data-ttu-id="fdb8c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fdb8c-122">Name</span></span>|<span data-ttu-id="fdb8c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb8c-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fdb8c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdb8c-124">Authorization</span></span>|<span data-ttu-id="fdb8c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdb8c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb8c-127">Request body</span></span>

<span data-ttu-id="fdb8c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdb8c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb8c-129">Response</span></span>

<span data-ttu-id="fdb8c-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos identityUserFlowAttribute](../resources/identityuserflowattribute.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdb8c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdb8c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdb8c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb8c-132">Request</span></span>

<span data-ttu-id="fdb8c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes
```

### <a name="response"></a><span data-ttu-id="fdb8c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb8c-134">Response</span></span>

<span data-ttu-id="fdb8c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-135">The following is an example of the response.</span></span>

<span data-ttu-id="fdb8c-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fdb8c-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
