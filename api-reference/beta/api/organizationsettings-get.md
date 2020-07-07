---
title: Obter organizationSettings
description: Recupere as propriedades e os relacionamentos do objeto organizationSettings.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 240704fd29f3950060342f4d2b8ab2efcc6f2ee0
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051007"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="5ee33-103">Obter organizationSettings</span><span class="sxs-lookup"><span data-stu-id="5ee33-103">Get organizationSettings</span></span>

<span data-ttu-id="5ee33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee33-105">Recupere as propriedades e os relacionamentos de um objeto [organizationSettings](../resources/organizationsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="5ee33-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ee33-106">Permissions</span></span>

<span data-ttu-id="5ee33-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5ee33-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5ee33-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee33-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ee33-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee33-109">Permission type</span></span>                        | <span data-ttu-id="5ee33-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ee33-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ee33-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ee33-112">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="5ee33-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="5ee33-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ee33-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee33-114">Not supported.</span></span>                              |
| <span data-ttu-id="5ee33-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee33-115">Application</span></span>                            | <span data-ttu-id="5ee33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee33-116">Not supported.</span></span>                              |

><span data-ttu-id="5ee33-117">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="5ee33-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ee33-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee33-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ee33-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ee33-119">Optional query parameters</span></span>

<span data-ttu-id="5ee33-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee33-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ee33-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ee33-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ee33-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee33-122">Request headers</span></span>

| <span data-ttu-id="5ee33-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5ee33-123">Name</span></span>          |<span data-ttu-id="5ee33-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee33-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="5ee33-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee33-125">Authorization</span></span> | <span data-ttu-id="5ee33-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5ee33-126">Bearer {token}.</span></span> <span data-ttu-id="5ee33-127">Required.</span><span class="sxs-lookup"><span data-stu-id="5ee33-127">Required.</span></span>   |
| <span data-ttu-id="5ee33-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ee33-128">Content-Type</span></span>  | <span data-ttu-id="5ee33-129">application/json.</span><span class="sxs-lookup"><span data-stu-id="5ee33-129">application/json.</span></span> <span data-ttu-id="5ee33-130">Required.</span><span class="sxs-lookup"><span data-stu-id="5ee33-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ee33-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee33-131">Request body</span></span>

<span data-ttu-id="5ee33-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ee33-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ee33-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee33-133">Response</span></span>

<span data-ttu-id="5ee33-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationSettings](../resources/organizationsettings.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee33-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ee33-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ee33-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ee33-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee33-136">Request</span></span>

<span data-ttu-id="5ee33-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee33-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

### <a name="response"></a><span data-ttu-id="5ee33-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee33-138">Response</span></span>

<span data-ttu-id="5ee33-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee33-139">The following is an example of the response.</span></span>

> <span data-ttu-id="5ee33-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5ee33-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5ee33-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5ee33-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "345233-676277-644334-445677-334556",
  "profileCardProperties": [
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
  "description": "Get organizationSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
