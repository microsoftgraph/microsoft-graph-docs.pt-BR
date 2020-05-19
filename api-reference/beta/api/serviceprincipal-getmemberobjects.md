---
title: 'servicePrincipalName: getMemberObjects'
description: Obtenha a lista de grupos e funções de diretório dos quais essa entidade de serviço é membro.  Essa verificação é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ec9fb6a3f70c02ac7abc2770c8cba481466f7f0c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291248"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="da792-104">servicePrincipalName: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="da792-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="da792-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da792-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da792-106">Obtenha a lista de grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="da792-106">Get the list of groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="da792-107">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="da792-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="da792-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="da792-108">Permissions</span></span>
<span data-ttu-id="da792-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da792-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da792-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da792-111">Permission type</span></span>      | <span data-ttu-id="da792-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da792-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da792-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da792-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da792-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da792-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da792-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da792-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da792-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da792-116">Not supported.</span></span>    |
|<span data-ttu-id="da792-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da792-117">Application</span></span> | <span data-ttu-id="da792-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da792-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da792-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da792-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="da792-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da792-120">Request headers</span></span>
| <span data-ttu-id="da792-121">Nome</span><span class="sxs-lookup"><span data-stu-id="da792-121">Name</span></span>       | <span data-ttu-id="da792-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="da792-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="da792-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da792-123">Authorization</span></span> | <span data-ttu-id="da792-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da792-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da792-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="da792-126">Content-type</span></span> | <span data-ttu-id="da792-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da792-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da792-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da792-129">Request body</span></span>
<span data-ttu-id="da792-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da792-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da792-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="da792-131">Parameter</span></span>    | <span data-ttu-id="da792-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="da792-132">Type</span></span>   |<span data-ttu-id="da792-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="da792-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da792-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="da792-134">securityEnabledOnly</span></span>|<span data-ttu-id="da792-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="da792-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="da792-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da792-136">Response</span></span>

<span data-ttu-id="da792-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da792-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da792-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da792-138">Examples</span></span>
<span data-ttu-id="da792-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="da792-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="da792-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da792-140">Request</span></span>
<span data-ttu-id="da792-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da792-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

### <a name="response"></a><span data-ttu-id="da792-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="da792-142">Response</span></span>
<span data-ttu-id="da792-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da792-143">Here is an example of the response.</span></span> 
><span data-ttu-id="da792-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da792-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
