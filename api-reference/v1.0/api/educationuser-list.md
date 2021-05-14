---
title: Listar educationUser
description: Obter uma lista dos objetos educationUser e suas propriedades.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6cf915d28369314d960ee4b868bafd2852819c7f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475370"
---
# <a name="list-educationusers"></a><span data-ttu-id="1599c-103">Listar educationUsers</span><span class="sxs-lookup"><span data-stu-id="1599c-103">List educationUsers</span></span>

<span data-ttu-id="1599c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1599c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1599c-105">Obter uma lista dos [objetos educationUser](../resources/educationuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1599c-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1599c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1599c-106">Permissions</span></span>

<span data-ttu-id="1599c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1599c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1599c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1599c-109">Permission type</span></span>                        | <span data-ttu-id="1599c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1599c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1599c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1599c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1599c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1599c-112">Not supported.</span></span>                              |
| <span data-ttu-id="1599c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1599c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1599c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1599c-114">Not supported.</span></span>                              |
| <span data-ttu-id="1599c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1599c-115">Application</span></span>                            | <span data-ttu-id="1599c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1599c-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1599c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1599c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1599c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1599c-118">Optional query parameters</span></span>

<span data-ttu-id="1599c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1599c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="1599c-120">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="1599c-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1599c-121">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="1599c-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="1599c-122">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1599c-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1599c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1599c-123">Request headers</span></span>

| <span data-ttu-id="1599c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1599c-124">Name</span></span>          | <span data-ttu-id="1599c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1599c-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1599c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1599c-126">Authorization</span></span> | <span data-ttu-id="1599c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1599c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1599c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1599c-129">Request body</span></span>

<span data-ttu-id="1599c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1599c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1599c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1599c-131">Response</span></span>

<span data-ttu-id="1599c-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1599c-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1599c-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1599c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1599c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1599c-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1599c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1599c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="1599c-136">C#</span><span class="sxs-lookup"><span data-stu-id="1599c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1599c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1599c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1599c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1599c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1599c-139">Java</span><span class="sxs-lookup"><span data-stu-id="1599c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1599c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1599c-140">Response</span></span>

> <span data-ttu-id="1599c-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1599c-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
