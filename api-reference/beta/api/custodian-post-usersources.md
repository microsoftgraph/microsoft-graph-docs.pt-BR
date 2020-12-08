---
title: Criar usuário
description: Criar um novo objeto username.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9ff054926611c990f8db0a2f868ac3449708436f
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597481"
---
# <a name="create-usersource"></a><span data-ttu-id="7c224-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="7c224-103">Create userSource</span></span>

<span data-ttu-id="7c224-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7c224-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c224-105">Criar um novo objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="7c224-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c224-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7c224-106">Permissions</span></span>

<span data-ttu-id="7c224-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c224-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c224-109">Permission type</span></span>|<span data-ttu-id="7c224-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c224-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c224-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c224-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c224-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="7c224-112">User.Read</span></span>|
|<span data-ttu-id="7c224-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c224-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c224-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c224-114">Not supported.</span></span>|
|<span data-ttu-id="7c224-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c224-115">Application</span></span>|<span data-ttu-id="7c224-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c224-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c224-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c224-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="7c224-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c224-118">Request headers</span></span>

|<span data-ttu-id="7c224-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7c224-119">Name</span></span>|<span data-ttu-id="7c224-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c224-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c224-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c224-121">Authorization</span></span>|<span data-ttu-id="7c224-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c224-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c224-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c224-124">Content-Type</span></span>|<span data-ttu-id="7c224-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c224-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c224-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c224-127">Request body</span></span>

<span data-ttu-id="7c224-128">No corpo da solicitação, forneça uma representação JSON do objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="7c224-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="7c224-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [username](../resources/usersource.md).</span><span class="sxs-lookup"><span data-stu-id="7c224-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="7c224-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c224-130">Property</span></span>|<span data-ttu-id="7c224-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c224-131">Type</span></span>|<span data-ttu-id="7c224-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c224-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c224-133">email</span><span class="sxs-lookup"><span data-stu-id="7c224-133">email</span></span>|<span data-ttu-id="7c224-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c224-134">String</span></span>|<span data-ttu-id="7c224-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="7c224-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="7c224-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="7c224-136">includedSources</span></span>|<span data-ttu-id="7c224-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="7c224-137">sourceType</span></span>|<span data-ttu-id="7c224-138">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="7c224-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="7c224-139">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="7c224-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="7c224-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c224-140">Response</span></span>

<span data-ttu-id="7c224-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [username](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c224-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c224-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7c224-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c224-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c224-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="7c224-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c224-144">Response</span></span>

<span data-ttu-id="7c224-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c224-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
