---
title: Listar mobileAppManagementPolicies
description: Obter uma lista dos objetos de política de gerenciamento de aplicativo móvel e suas propriedades.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3c50e81c1e7d49f55eafa1eb7b0b5ece32e05a68
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401656"
---
# <a name="list-mobileappmanagementpolicies"></a><span data-ttu-id="47e72-103">Listar mobileAppManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="47e72-103">List mobileAppManagementPolicies</span></span>

<span data-ttu-id="47e72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e72-105">Obter uma lista dos [objetos mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="47e72-105">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="47e72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47e72-106">Permissions</span></span>

<span data-ttu-id="47e72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47e72-109">Permission type</span></span>|<span data-ttu-id="47e72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47e72-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47e72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47e72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47e72-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="47e72-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="47e72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47e72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47e72-114">Not supported.</span></span>|
|<span data-ttu-id="47e72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47e72-115">Application</span></span> | <span data-ttu-id="47e72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47e72-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47e72-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47e72-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47e72-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47e72-118">Optional query parameters</span></span>

<span data-ttu-id="47e72-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47e72-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="47e72-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="47e72-120">For example:</span></span>

- <span data-ttu-id="47e72-121">Para selecionar atributos específicos, adicione `$select=id,displayname` .</span><span class="sxs-lookup"><span data-stu-id="47e72-121">To select specific attributes add `$select=id,displayname`.</span></span>
- <span data-ttu-id="47e72-122">Para recuperar grupos incluídos para cada política, adicione `$expand=includedGroups` .</span><span class="sxs-lookup"><span data-stu-id="47e72-122">To retrieve included groups for each policy, add `$expand=includedGroups`.</span></span>
- <span data-ttu-id="47e72-123">Para filtrar com base em um atributo, use `$filter=displayName eq 'Microsoft Intune'` .</span><span class="sxs-lookup"><span data-stu-id="47e72-123">To filter based on an attribute, use `$filter=displayName eq 'Microsoft Intune'`.</span></span>

<span data-ttu-id="47e72-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47e72-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47e72-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47e72-125">Request headers</span></span>

|<span data-ttu-id="47e72-126">Nome</span><span class="sxs-lookup"><span data-stu-id="47e72-126">Name</span></span>|<span data-ttu-id="47e72-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e72-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47e72-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="47e72-128">Authorization</span></span>|<span data-ttu-id="47e72-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47e72-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47e72-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47e72-131">Request body</span></span>

<span data-ttu-id="47e72-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47e72-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47e72-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="47e72-133">Response</span></span>

<span data-ttu-id="47e72-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47e72-134">If successful, this method returns a `200 OK` response code and a collection of [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47e72-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47e72-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47e72-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47e72-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies
```

### <a name="response"></a><span data-ttu-id="47e72-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="47e72-137">Response</span></span>

><span data-ttu-id="47e72-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47e72-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
   {
    "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.manage.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.manage.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.manage.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
  ]
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "List mobileAppManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
