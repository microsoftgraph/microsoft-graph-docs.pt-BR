---
title: 'informationProtectionLabel: listLabels'
description: Recupere uma lista de rótulos de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 07d1c8259603fff34f9f63860a558fc337a8af48
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938515"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="de61b-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="de61b-103">informationProtectionLabel: listLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de61b-104">Obtenha um conjunto de [Rótulos de proteção de informações](../resources/informationprotectionlabel.md) disponíveis para o usuário ou para a organização.</span><span class="sxs-lookup"><span data-stu-id="de61b-104">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="de61b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de61b-105">Permissions</span></span>

<span data-ttu-id="de61b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de61b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de61b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de61b-108">Permission type</span></span>                        | <span data-ttu-id="de61b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de61b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="de61b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de61b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de61b-111">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="de61b-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="de61b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de61b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de61b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de61b-113">Not supported.</span></span>                              |
| <span data-ttu-id="de61b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de61b-114">Application</span></span>                            | <span data-ttu-id="de61b-115">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="de61b-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="de61b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de61b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de61b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de61b-117">Optional query parameters</span></span>

<span data-ttu-id="de61b-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de61b-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="de61b-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="de61b-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="de61b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de61b-120">Request headers</span></span>

| <span data-ttu-id="de61b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de61b-121">Name</span></span>          | <span data-ttu-id="de61b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de61b-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="de61b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de61b-123">Authorization</span></span> | <span data-ttu-id="de61b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de61b-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="de61b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de61b-126">Request body</span></span>

<span data-ttu-id="de61b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de61b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de61b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="de61b-128">Response</span></span>

<span data-ttu-id="de61b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [informationProtectionLabel](../resources/informationprotectionlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de61b-129">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de61b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de61b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de61b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de61b-131">Request</span></span>

<span data-ttu-id="de61b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de61b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```http
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```

### <a name="response"></a><span data-ttu-id="de61b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="de61b-133">Response</span></span>

<span data-ttu-id="de61b-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de61b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="de61b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de61b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels",
  "value": [
      {
          "id": "3a80e051-487c-40d4-b491-73ad25d997e6",
          "name": "General",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 1,
          "tooltip": "Data classified as Contoso General.",
          "isActive": true
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List labels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
