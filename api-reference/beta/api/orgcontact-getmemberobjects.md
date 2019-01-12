---
title: 'orgContact: getMemberObjects'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 597dfeaa1870aab74d8bc813b50aebc2891dc430
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938850"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="48981-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="48981-104">orgContact: getMemberObjects</span></span>

> <span data-ttu-id="48981-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="48981-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48981-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="48981-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="48981-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="48981-107">Permissions</span></span>
<span data-ttu-id="48981-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48981-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48981-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48981-110">Permission type</span></span>      | <span data-ttu-id="48981-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48981-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48981-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48981-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48981-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48981-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48981-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48981-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48981-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48981-115">Not supported.</span></span>    |
|<span data-ttu-id="48981-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48981-116">Application</span></span> | <span data-ttu-id="48981-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48981-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48981-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48981-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="48981-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48981-119">Request headers</span></span>
| <span data-ttu-id="48981-120">Nome</span><span class="sxs-lookup"><span data-stu-id="48981-120">Name</span></span>       | <span data-ttu-id="48981-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="48981-121">Type</span></span> | <span data-ttu-id="48981-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="48981-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48981-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="48981-123">Authorization</span></span>  | <span data-ttu-id="48981-124">string</span><span class="sxs-lookup"><span data-stu-id="48981-124">string</span></span>  | <span data-ttu-id="48981-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48981-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48981-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48981-127">Request body</span></span>
<span data-ttu-id="48981-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48981-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48981-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="48981-129">Parameter</span></span>    | <span data-ttu-id="48981-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="48981-130">Type</span></span>   |<span data-ttu-id="48981-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="48981-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48981-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="48981-132">securityEnabledOnly</span></span>|<span data-ttu-id="48981-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="48981-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="48981-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="48981-134">Response</span></span>

<span data-ttu-id="48981-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48981-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48981-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48981-136">Example</span></span>
<span data-ttu-id="48981-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="48981-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48981-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48981-138">Request</span></span>
<span data-ttu-id="48981-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48981-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="48981-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="48981-140">Response</span></span>
<span data-ttu-id="48981-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48981-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
