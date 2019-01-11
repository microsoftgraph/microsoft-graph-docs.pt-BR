---
title: Listar os modelos existentes de sincronização
description: Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.
localization_priority: Normal
ms.openlocfilehash: 49e9e257322886fe294807207276f8b6d6919909
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839435"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="e5538-103">Listar os modelos existentes de sincronização</span><span class="sxs-lookup"><span data-stu-id="e5538-103">List existing synchronization templates</span></span>

> <span data-ttu-id="e5538-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5538-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5538-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5538-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5538-106">Lista os modelos de sincronização associados a um determinado aplicativo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e5538-106">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5538-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e5538-107">Permissions</span></span>
<span data-ttu-id="e5538-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5538-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5538-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5538-110">Permission type</span></span>                        | <span data-ttu-id="e5538-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5538-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5538-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5538-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="e5538-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5538-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e5538-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5538-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e5538-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5538-115">Not supported.</span></span>|
|<span data-ttu-id="e5538-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5538-116">Application</span></span>                            |<span data-ttu-id="e5538-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5538-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="e5538-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5538-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="e5538-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5538-119">Request headers</span></span>

| <span data-ttu-id="e5538-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e5538-120">Name</span></span>           | <span data-ttu-id="e5538-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5538-121">Type</span></span>    | <span data-ttu-id="e5538-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5538-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e5538-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5538-123">Authorization</span></span>  | <span data-ttu-id="e5538-124">string</span><span class="sxs-lookup"><span data-stu-id="e5538-124">string</span></span>  | <span data-ttu-id="e5538-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5538-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5538-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5538-127">Request body</span></span>

<span data-ttu-id="e5538-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5538-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e5538-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5538-129">Response</span></span>

<span data-ttu-id="e5538-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e acollection dos objetos [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5538-130">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="e5538-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5538-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e5538-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5538-132">Request</span></span>
<span data-ttu-id="e5538-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5538-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="e5538-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5538-134">Response</span></span>
<span data-ttu-id="e5538-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e5538-135">The following is an example of a response.</span></span>
><span data-ttu-id="e5538-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5538-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5538-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5538-137">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
