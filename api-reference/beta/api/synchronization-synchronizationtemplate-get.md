---
title: Obter synchronizationTemplate
description: Recupere um modelo de sincronização por seu identificador.
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524370"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="d534b-103">Obter synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="d534b-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d534b-104">Recupere um modelo de sincronização por seu identificador.</span><span class="sxs-lookup"><span data-stu-id="d534b-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="d534b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d534b-105">Permissions</span></span>
<span data-ttu-id="d534b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d534b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d534b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d534b-108">Permission type</span></span>                        | <span data-ttu-id="d534b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d534b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d534b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d534b-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="d534b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d534b-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d534b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d534b-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d534b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d534b-113">Not supported.</span></span>|
|<span data-ttu-id="d534b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d534b-114">Application</span></span>                            |<span data-ttu-id="d534b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d534b-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="d534b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d534b-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="d534b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d534b-117">Request headers</span></span>

| <span data-ttu-id="d534b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d534b-118">Name</span></span>           | <span data-ttu-id="d534b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d534b-119">Type</span></span>    | <span data-ttu-id="d534b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d534b-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d534b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d534b-121">Authorization</span></span>  | <span data-ttu-id="d534b-122">string</span><span class="sxs-lookup"><span data-stu-id="d534b-122">string</span></span>  | <span data-ttu-id="d534b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d534b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d534b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d534b-125">Request body</span></span>

<span data-ttu-id="d534b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d534b-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d534b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d534b-127">Response</span></span>

<span data-ttu-id="d534b-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d534b-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="d534b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d534b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d534b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d534b-130">Request</span></span>
<span data-ttu-id="d534b-131">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d534b-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="d534b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d534b-132">Response</span></span>
<span data-ttu-id="d534b-133">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d534b-133">The following is an example of a response.</span></span>
><span data-ttu-id="d534b-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d534b-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d534b-135">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d534b-135">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
