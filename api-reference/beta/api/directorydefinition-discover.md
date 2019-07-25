---
title: 'directoryDefinition: descobrir'
description: 'Descubra a definição de esquema mais recente para provisionamento para um aplicativo. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aafd4ad57d8e6d75ebdcd3c7bf2fba4506e48f56
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879574"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="32964-103">directoryDefinition: descobrir</span><span class="sxs-lookup"><span data-stu-id="32964-103">directoryDefinition: discover</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32964-104">Descubra a definição de esquema mais recente para provisionamento para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32964-104">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="32964-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="32964-105">Permissions</span></span>

<span data-ttu-id="32964-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32964-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32964-108">Permission type</span></span>                        | <span data-ttu-id="32964-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32964-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="32964-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32964-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="32964-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32964-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="32964-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32964-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32964-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32964-113">Not supported.</span></span> |
| <span data-ttu-id="32964-114">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="32964-114">Application-only</span></span>                            | <span data-ttu-id="32964-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32964-115">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32964-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32964-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="32964-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32964-117">Request headers</span></span>

| <span data-ttu-id="32964-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32964-118">Header</span></span>        | <span data-ttu-id="32964-119">Valor</span><span class="sxs-lookup"><span data-stu-id="32964-119">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="32964-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="32964-120">Authorization</span></span> | <span data-ttu-id="32964-121">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="32964-121">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32964-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32964-122">Request body</span></span>

<span data-ttu-id="32964-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32964-123">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="32964-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="32964-124">Response</span></span>

<span data-ttu-id="32964-125">Se tiver êxito, este método retornará `200 OK` uma resposta com um objeto [directoryDefinition](../resources/synchronization-directorydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="32964-125">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="32964-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32964-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="32964-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32964-127">Request</span></span>
<span data-ttu-id="32964-128">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="32964-128">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

### <a name="response"></a><span data-ttu-id="32964-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32964-129">Response</span></span>

<span data-ttu-id="32964-130">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="32964-130">The following is an example of a response.</span></span>

><span data-ttu-id="32964-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32964-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```
