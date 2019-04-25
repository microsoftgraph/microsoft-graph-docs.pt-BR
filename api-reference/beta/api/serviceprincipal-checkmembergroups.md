---
title: 'servicePrincipalName: checkMemberGroups'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
ms.openlocfilehash: 2237f83ce32bbb34f983226011f1c324185040b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545515"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="fab85-104">servicePrincipalName: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fab85-104">servicePrincipal: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="fab85-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fab85-105">Permissions</span></span>
<span data-ttu-id="fab85-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab85-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fab85-108">Permission type</span></span>      | <span data-ttu-id="fab85-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fab85-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fab85-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fab85-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fab85-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fab85-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fab85-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fab85-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fab85-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fab85-113">Not supported.</span></span>    |
|<span data-ttu-id="fab85-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fab85-114">Application</span></span> | <span data-ttu-id="fab85-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fab85-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fab85-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fab85-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="fab85-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fab85-117">Request headers</span></span>
| <span data-ttu-id="fab85-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fab85-118">Name</span></span>       | <span data-ttu-id="fab85-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab85-119">Type</span></span> | <span data-ttu-id="fab85-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab85-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fab85-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fab85-121">Authorization</span></span>  | <span data-ttu-id="fab85-122">string</span><span class="sxs-lookup"><span data-stu-id="fab85-122">string</span></span>  | <span data-ttu-id="fab85-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fab85-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fab85-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fab85-125">Request body</span></span>
<span data-ttu-id="fab85-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab85-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fab85-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fab85-127">Parameter</span></span>    | <span data-ttu-id="fab85-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab85-128">Type</span></span>   |<span data-ttu-id="fab85-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab85-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fab85-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="fab85-130">groupIds</span></span>|<span data-ttu-id="fab85-131">String</span><span class="sxs-lookup"><span data-stu-id="fab85-131">String</span></span>||

## <a name="response"></a><span data-ttu-id="fab85-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab85-132">Response</span></span>

<span data-ttu-id="fab85-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fab85-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab85-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fab85-134">Example</span></span>
<span data-ttu-id="fab85-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fab85-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fab85-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fab85-136">Request</span></span>
<span data-ttu-id="fab85-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab85-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="fab85-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab85-138">Response</span></span>
<span data-ttu-id="fab85-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fab85-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
