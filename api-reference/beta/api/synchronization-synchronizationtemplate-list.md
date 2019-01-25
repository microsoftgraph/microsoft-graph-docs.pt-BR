---
title: Listar os modelos existentes de sincronização
description: Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 309d1ddd6d702652b14e10895de10486a5d23783
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523628"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="11d35-103">Listar os modelos existentes de sincronização</span><span class="sxs-lookup"><span data-stu-id="11d35-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d35-104">Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="11d35-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="11d35-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="11d35-105">Permissions</span></span>
<span data-ttu-id="11d35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11d35-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11d35-108">Permission type</span></span>                        | <span data-ttu-id="11d35-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11d35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="11d35-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11d35-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="11d35-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11d35-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="11d35-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11d35-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="11d35-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11d35-113">Not supported.</span></span>|
|<span data-ttu-id="11d35-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11d35-114">Application</span></span>                            |<span data-ttu-id="11d35-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11d35-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="11d35-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11d35-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="11d35-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11d35-117">Request headers</span></span>

| <span data-ttu-id="11d35-118">Nome</span><span class="sxs-lookup"><span data-stu-id="11d35-118">Name</span></span>           | <span data-ttu-id="11d35-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="11d35-119">Type</span></span>    | <span data-ttu-id="11d35-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d35-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="11d35-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="11d35-121">Authorization</span></span>  | <span data-ttu-id="11d35-122">string</span><span class="sxs-lookup"><span data-stu-id="11d35-122">string</span></span>  | <span data-ttu-id="11d35-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11d35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11d35-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11d35-125">Request body</span></span>

<span data-ttu-id="11d35-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11d35-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="11d35-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d35-127">Response</span></span>

<span data-ttu-id="11d35-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e acollection dos objetos [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11d35-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="11d35-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11d35-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="11d35-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11d35-130">Request</span></span>
<span data-ttu-id="11d35-131">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="11d35-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="11d35-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11d35-132">Response</span></span>
<span data-ttu-id="11d35-133">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="11d35-133">The following is an example of a response.</span></span>
><span data-ttu-id="11d35-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11d35-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="11d35-135">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11d35-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
