---
title: Criar esquema
description: Crie o esquema para uma Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 98c4c83ff8a8712905ace9fa80ec4fdae0de7180
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467209"
---
# <a name="create-schema"></a><span data-ttu-id="3dba4-103">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="3dba4-103">Create schema</span></span>
<span data-ttu-id="3dba4-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="3dba4-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="3dba4-105">Crie um novo [objeto de esquema.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="3dba4-105">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dba4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dba4-106">Permissions</span></span>
<span data-ttu-id="3dba4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dba4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dba4-109">Permission type</span></span>|<span data-ttu-id="3dba4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dba4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dba4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dba4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3dba4-112">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="3dba4-112">Not applicable</span></span>|
|<span data-ttu-id="3dba4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dba4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dba4-114">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="3dba4-114">Not applicable</span></span>|
|<span data-ttu-id="3dba4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dba4-115">Application</span></span>| <span data-ttu-id="3dba4-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="3dba4-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dba4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dba4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
<span data-ttu-id="3dba4-118">No corpo da solicitação, fornece uma representação JSON de um [objeto de esquema.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="3dba4-118">In the request body, supply a JSON representation of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

<span data-ttu-id="3dba4-119">Ao registrar um esquema de item personalizado, o objeto DEVE ter a propriedade `schema` definida como e DEVE conter a `baseType` `microsoft.graph.externalItem` `properties` propriedade.</span><span class="sxs-lookup"><span data-stu-id="3dba4-119">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="3dba4-120">O `properties` objeto deve conter pelo menos uma propriedade, até um máximo de 64.</span><span class="sxs-lookup"><span data-stu-id="3dba4-120">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="3dba4-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dba4-121">Response</span></span>

<span data-ttu-id="3dba4-122">Com o header incluído na solicitação, se bem-sucedido, este método retorna um código de resposta e uma URL no header de resposta que podem ser usados para obter o `Prefer: respond-async` `202 Accepted` status da `Location` [operação](../api/externalconnectors-connectionoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="3dba4-122">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/externalconnectors-connectionoperation-get.md).</span></span>

<span data-ttu-id="3dba4-123">Sem o header incluído na solicitação, se bem-sucedido, este método retorna um código de resposta e um novo objeto `Prefer: respond-async` de esquema no corpo da `201 Created` resposta. [](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="3dba4-123">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="3dba4-124">A criação de um esquema é um processo de longa duração propenso a tempos-de-tempo de gateway.</span><span class="sxs-lookup"><span data-stu-id="3dba4-124">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="3dba4-125">Recomendamos usar `Prefer: respond-async` o header para evitar erros de tempo de tempo.</span><span class="sxs-lookup"><span data-stu-id="3dba4-125">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="3dba4-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3dba4-126">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="3dba4-127">Exemplo: Registrar esquema personalizado de forma assíncrona</span><span class="sxs-lookup"><span data-stu-id="3dba4-127">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="3dba4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dba4-128">Request</span></span>

<span data-ttu-id="3dba4-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dba4-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dba4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dba4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="3dba4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dba4-131">Response</span></span>

<span data-ttu-id="3dba4-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3dba4-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
