---
title: Listar profileCardProperties
description: Recupere uma lista de objetos profilecardproperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4aa23e69308d8c13cc9ceb25bcc1398c9cbb1012
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051006"
---
# <a name="list-profilecardproperties"></a><span data-ttu-id="fe751-103">Listar profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="fe751-103">List profileCardProperties</span></span>

<span data-ttu-id="fe751-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe751-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe751-105">Obtenha uma coleção de recursos [profileCardProperty](../resources/profilecardproperty.md) de uma organização.</span><span class="sxs-lookup"><span data-stu-id="fe751-105">Get a collection of [profileCardProperty](../resources/profilecardproperty.md) resources of an organization.</span></span> <span data-ttu-id="fe751-106">Cada recurso é identificado pela propriedade **directoryPropertyName** .</span><span class="sxs-lookup"><span data-stu-id="fe751-106">Each resource is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe751-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe751-107">Permissions</span></span>

<span data-ttu-id="fe751-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fe751-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fe751-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe751-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe751-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe751-110">Permission type</span></span>                        | <span data-ttu-id="fe751-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe751-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fe751-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe751-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe751-113">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="fe751-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="fe751-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe751-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe751-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe751-115">Not supported.</span></span>                              |
| <span data-ttu-id="fe751-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe751-116">Application</span></span>                            | <span data-ttu-id="fe751-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe751-117">Not supported.</span></span>                              |

><span data-ttu-id="fe751-118">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="fe751-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="fe751-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe751-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe751-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe751-120">Optional query parameters</span></span>

<span data-ttu-id="fe751-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe751-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fe751-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fe751-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe751-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe751-123">Request headers</span></span>

| <span data-ttu-id="fe751-124">Nome</span><span class="sxs-lookup"><span data-stu-id="fe751-124">Name</span></span>          |<span data-ttu-id="fe751-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe751-125">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="fe751-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe751-126">Authorization</span></span> | <span data-ttu-id="fe751-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fe751-127">Bearer {token}.</span></span> <span data-ttu-id="fe751-128">Required.</span><span class="sxs-lookup"><span data-stu-id="fe751-128">Required.</span></span>   |
| <span data-ttu-id="fe751-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe751-129">Content-Type</span></span>  | <span data-ttu-id="fe751-130">application/json.</span><span class="sxs-lookup"><span data-stu-id="fe751-130">application/json.</span></span> <span data-ttu-id="fe751-131">Required.</span><span class="sxs-lookup"><span data-stu-id="fe751-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe751-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe751-132">Request body</span></span>

<span data-ttu-id="fe751-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe751-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe751-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe751-134">Response</span></span>

<span data-ttu-id="fe751-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [profileCardProperty](../resources/profilecardproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe751-135">If successful, this method returns a `200 OK` response code and a collection of [profileCardProperty](../resources/profilecardproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe751-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe751-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe751-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe751-137">Request</span></span>

<span data-ttu-id="fe751-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe751-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

### <a name="response"></a><span data-ttu-id="fe751-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe751-139">Response</span></span>

<span data-ttu-id="fe751-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe751-140">The following is an example of the response.</span></span>

> <span data-ttu-id="fe751-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fe751-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe751-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fe751-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "directoryPropertyName": "CustomAttribute1",
      "annotations": [
        {
          "displayName": "Cost Center",
          "localizations": [
            {
              "languageTag": "ru-RU",
              "displayName": "центр затрат"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List profileCardProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
