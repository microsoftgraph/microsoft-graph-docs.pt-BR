---
title: 'orgContact: checkMemberGroups'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
ms.openlocfilehash: d064775772bb05963e3cd789346e32bf80b7587c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037053"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="8cc74-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8cc74-104">orgContact: checkMemberGroups</span></span>

> <span data-ttu-id="8cc74-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8cc74-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cc74-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8cc74-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc74-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8cc74-107">Permissions</span></span>
<span data-ttu-id="8cc74-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc74-110">Permission type</span></span>      | <span data-ttu-id="8cc74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc74-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cc74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc74-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cc74-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cc74-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cc74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc74-115">Not supported.</span></span>    |
|<span data-ttu-id="8cc74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc74-116">Application</span></span> | <span data-ttu-id="8cc74-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc74-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc74-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="8cc74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc74-119">Request headers</span></span>
| <span data-ttu-id="8cc74-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc74-120">Name</span></span>       | <span data-ttu-id="8cc74-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc74-121">Type</span></span> | <span data-ttu-id="8cc74-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc74-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8cc74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc74-123">Authorization</span></span>  | <span data-ttu-id="8cc74-124">string</span><span class="sxs-lookup"><span data-stu-id="8cc74-124">string</span></span>  | <span data-ttu-id="8cc74-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc74-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc74-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc74-127">Request body</span></span>
<span data-ttu-id="8cc74-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc74-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cc74-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8cc74-129">Parameter</span></span>    | <span data-ttu-id="8cc74-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc74-130">Type</span></span>   |<span data-ttu-id="8cc74-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc74-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cc74-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="8cc74-132">groupIds</span></span>|<span data-ttu-id="8cc74-133">String</span><span class="sxs-lookup"><span data-stu-id="8cc74-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="8cc74-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc74-134">Response</span></span>

<span data-ttu-id="8cc74-135">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc74-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc74-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc74-136">Example</span></span>
<span data-ttu-id="8cc74-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8cc74-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cc74-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc74-138">Request</span></span>
<span data-ttu-id="8cc74-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc74-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8cc74-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc74-140">Response</span></span>
<span data-ttu-id="8cc74-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc74-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->