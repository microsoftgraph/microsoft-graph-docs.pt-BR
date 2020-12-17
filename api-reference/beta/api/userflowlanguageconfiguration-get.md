---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e os relacionamentos de um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) .
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d25533822a5f67cdfc98564a41e7f53b3be98208
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706221"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="38730-103">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="38730-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="38730-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38730-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38730-105">Leia as propriedades e os relacionamentos de um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="38730-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="38730-106">Esses objetos representam um idioma disponível em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="38730-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="38730-107">**Observação:** Para recuperar um idioma com suporte para personalização, você deve primeiro habilitar a personalização de idioma em seu fluxo de usuário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="38730-107">**Note:** To retrieve a language supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="38730-108">Para obter mais informações, consulte [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span><span class="sxs-lookup"><span data-stu-id="38730-108">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span> <span data-ttu-id="38730-109">A personalização de idioma é habilitada por padrão em [fluxos de usuário do Azure Active Directory](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="38730-109">Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38730-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="38730-110">Permissions</span></span>

<span data-ttu-id="38730-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38730-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38730-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38730-113">Permission type</span></span>      | <span data-ttu-id="38730-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38730-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38730-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38730-115">Delegated (work or school account)</span></span>|<span data-ttu-id="38730-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="38730-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="38730-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38730-117">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="38730-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38730-118">Not supported.</span></span>|
|<span data-ttu-id="38730-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38730-119">Application</span></span>|<span data-ttu-id="38730-120">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="38730-120">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="38730-121">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="38730-121">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="38730-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="38730-122">Global administrator</span></span>
* <span data-ttu-id="38730-123">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="38730-123">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="38730-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38730-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/languages/{id}
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38730-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38730-125">Request headers</span></span>

|<span data-ttu-id="38730-126">Nome</span><span class="sxs-lookup"><span data-stu-id="38730-126">Name</span></span>|<span data-ttu-id="38730-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="38730-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="38730-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="38730-128">Authorization</span></span>|<span data-ttu-id="38730-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38730-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38730-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38730-131">Request body</span></span>

<span data-ttu-id="38730-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38730-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38730-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38730-133">Response</span></span>

<span data-ttu-id="38730-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38730-134">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38730-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38730-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38730-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38730-136">Request</span></span>

<span data-ttu-id="38730-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38730-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en
```

### <a name="response"></a><span data-ttu-id="38730-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="38730-138">Response</span></span>

<span data-ttu-id="38730-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38730-139">The following is an example of the response.</span></span>

<span data-ttu-id="38730-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="38730-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_Customer')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
