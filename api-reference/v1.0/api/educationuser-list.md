---
title: Listar educationUser
description: Obter uma lista dos objetos educationUser e suas propriedades.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fa8f0105257991ca5b7ea255d3ea3b534bb079b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232129"
---
# <a name="list-educationusers"></a><span data-ttu-id="e9561-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="e9561-103">List educationUsers</span></span>

<span data-ttu-id="e9561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9561-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9561-105">Obter uma lista dos [objetos educationUser](../resources/educationuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e9561-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9561-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9561-106">Permissions</span></span>

<span data-ttu-id="e9561-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9561-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9561-109">Permission type</span></span>                        | <span data-ttu-id="e9561-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9561-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e9561-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9561-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9561-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9561-112">Not supported.</span></span>                              |
| <span data-ttu-id="e9561-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9561-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9561-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9561-114">Not supported.</span></span>                              |
| <span data-ttu-id="e9561-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9561-115">Application</span></span>                            | <span data-ttu-id="e9561-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9561-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9561-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9561-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9561-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9561-118">Optional query parameters</span></span>

<span data-ttu-id="e9561-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e9561-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="e9561-120">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="e9561-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e9561-121">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="e9561-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="e9561-122">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e9561-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9561-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9561-123">Request headers</span></span>

| <span data-ttu-id="e9561-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e9561-124">Name</span></span>          | <span data-ttu-id="e9561-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9561-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e9561-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9561-126">Authorization</span></span> | <span data-ttu-id="e9561-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9561-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9561-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9561-129">Request body</span></span>

<span data-ttu-id="e9561-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9561-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9561-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9561-131">Response</span></span>

<span data-ttu-id="e9561-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9561-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9561-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e9561-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9561-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9561-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users
```

### <a name="response"></a><span data-ttu-id="e9561-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9561-135">Response</span></span>

> <span data-ttu-id="e9561-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e9561-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```
