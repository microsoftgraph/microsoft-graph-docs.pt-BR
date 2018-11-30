---
title: Obter synchronizationTemplate
description: Recupere um modelo de sincronização por seu identificador.
ms.openlocfilehash: 1ff3f11cf42f5a861e379c8fba2b491fbee2225e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035062"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="e98b1-103">Obter synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="e98b1-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="e98b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e98b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e98b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e98b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e98b1-106">Recupere um modelo de sincronização por seu identificador.</span><span class="sxs-lookup"><span data-stu-id="e98b1-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="e98b1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e98b1-107">Permissions</span></span>
<span data-ttu-id="e98b1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e98b1-110">Permission type</span></span>                        | <span data-ttu-id="e98b1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e98b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e98b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e98b1-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="e98b1-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98b1-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e98b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e98b1-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e98b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98b1-115">Not supported.</span></span>|
|<span data-ttu-id="e98b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e98b1-116">Application</span></span>                            |<span data-ttu-id="e98b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98b1-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="e98b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e98b1-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="e98b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e98b1-119">Request headers</span></span>

| <span data-ttu-id="e98b1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e98b1-120">Name</span></span>           | <span data-ttu-id="e98b1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e98b1-121">Type</span></span>    | <span data-ttu-id="e98b1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e98b1-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e98b1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e98b1-123">Authorization</span></span>  | <span data-ttu-id="e98b1-124">string</span><span class="sxs-lookup"><span data-stu-id="e98b1-124">string</span></span>  | <span data-ttu-id="e98b1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e98b1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e98b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e98b1-127">Request body</span></span>

<span data-ttu-id="e98b1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e98b1-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e98b1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98b1-129">Response</span></span>

<span data-ttu-id="e98b1-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e98b1-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="e98b1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e98b1-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e98b1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e98b1-132">Request</span></span>
<span data-ttu-id="e98b1-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e98b1-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="e98b1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98b1-134">Response</span></span>
<span data-ttu-id="e98b1-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e98b1-135">The following is an example of a response.</span></span>
><span data-ttu-id="e98b1-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e98b1-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e98b1-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e98b1-137">All the properties will be returned in an actual call.</span></span>

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