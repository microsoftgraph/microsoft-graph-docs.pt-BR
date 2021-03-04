---
title: Listar itens excluídos pertencentes a um usuário
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 31a85be8a5c6b1dc09889ea77cf619060f702789
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436978"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="31526-103">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="31526-103">List deleted items owned by a user</span></span>

<span data-ttu-id="31526-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31526-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31526-105">Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="31526-105">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="31526-106">Atualmente, a funcionalidade de itens excluídos de [](../resources/group.md) lista tem suporte apenas para [recursos](../resources/application.md) de aplicativo e grupo pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="31526-106">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="31526-107">Esta é uma ação de serviço, o que significa que ela não dá suporte à paginação.</span><span class="sxs-lookup"><span data-stu-id="31526-107">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="31526-108">A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificação por ID.</span><span class="sxs-lookup"><span data-stu-id="31526-108">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="31526-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="31526-109">Permissions</span></span>

<span data-ttu-id="31526-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31526-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31526-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31526-112">Permission type</span></span> | <span data-ttu-id="31526-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31526-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="31526-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31526-114">Delegated (work or school account)</span></span> | <span data-ttu-id="31526-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31526-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="31526-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31526-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="31526-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31526-117">Not supported.</span></span> |
| <span data-ttu-id="31526-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31526-118">Application</span></span> | <span data-ttu-id="31526-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31526-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="31526-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31526-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="31526-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31526-121">Request headers</span></span>

| <span data-ttu-id="31526-122">Nome</span><span class="sxs-lookup"><span data-stu-id="31526-122">Name</span></span>          | <span data-ttu-id="31526-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="31526-123">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="31526-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="31526-124">Authorization</span></span> | <span data-ttu-id="31526-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31526-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31526-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31526-127">Request body</span></span>

<span data-ttu-id="31526-128">O corpo da solicitação requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="31526-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="31526-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="31526-129">Parameter</span></span>    | <span data-ttu-id="31526-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="31526-130">Type</span></span> |<span data-ttu-id="31526-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="31526-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31526-132">userId</span><span class="sxs-lookup"><span data-stu-id="31526-132">userId</span></span>|<span data-ttu-id="31526-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31526-133">String</span></span>|<span data-ttu-id="31526-134">ID do proprietário.</span><span class="sxs-lookup"><span data-stu-id="31526-134">ID of the owner.</span></span>|
|<span data-ttu-id="31526-135">type</span><span class="sxs-lookup"><span data-stu-id="31526-135">type</span></span>|<span data-ttu-id="31526-136">String</span><span class="sxs-lookup"><span data-stu-id="31526-136">String</span></span>|<span data-ttu-id="31526-137">Tipo de objetos de propriedade a retornar; `group` atualmente é o único valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="31526-137">Type of owned objects to return; `group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="31526-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="31526-138">Response</span></span>

<span data-ttu-id="31526-139">Solicitações `200 OK` bem-sucedidas retornam códigos de resposta; o objeto de resposta inclui propriedades [de diretório (itens excluídos).](../resources/directory.md)</span><span class="sxs-lookup"><span data-stu-id="31526-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="31526-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31526-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="31526-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31526-141">Request</span></span>

<span data-ttu-id="31526-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31526-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="31526-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="31526-143">Response</span></span>

<span data-ttu-id="31526-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31526-144">Here is an example of the response.</span></span> <span data-ttu-id="31526-145">Observação: esse objeto de resposta pode ser truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="31526-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="31526-146">Todas as propriedades com suporte são retornadas de chamadas reais.</span><span class="sxs-lookup"><span data-stu-id="31526-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```
