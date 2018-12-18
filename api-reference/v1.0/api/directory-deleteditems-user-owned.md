---
title: Permissões
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
author: lleonard-msft
ms.openlocfilehash: 9ce487d957f4bdaa2684d00865aeac7ea293ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351167"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="b1c46-103">**Listar itens excluídos pertencentes a um usuário**</span><span class="sxs-lookup"><span data-stu-id="b1c46-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="b1c46-104">Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="b1c46-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="b1c46-105">Atualmente, a funcionalidade de itens de lista excluída é suportada somente para [Agrupar](../resources/group.md) recursos pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="b1c46-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="b1c46-106">Esta é uma ação de serviço, o que significa que ele não dá suporte a paginação.</span><span class="sxs-lookup"><span data-stu-id="b1c46-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="b1c46-107">A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificado por ID.</span><span class="sxs-lookup"><span data-stu-id="b1c46-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c46-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c46-108">Permissions</span></span>

<span data-ttu-id="b1c46-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="b1c46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="b1c46-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1c46-111">Permission type</span></span> | <span data-ttu-id="b1c46-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1c46-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="b1c46-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1c46-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1c46-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c46-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b1c46-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1c46-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b1c46-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c46-116">Not supported.</span></span> |
| <span data-ttu-id="b1c46-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1c46-117">Application</span></span> | <span data-ttu-id="b1c46-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1c46-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b1c46-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c46-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="b1c46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c46-120">Request headers</span></span>

| <span data-ttu-id="b1c46-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b1c46-121">Name</span></span>          | <span data-ttu-id="b1c46-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c46-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="b1c46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1c46-123">Authorization</span></span> | <span data-ttu-id="b1c46-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1c46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1c46-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c46-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="b1c46-127">O corpo da solicitação requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="b1c46-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="b1c46-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b1c46-128">Parameter</span></span>    | <span data-ttu-id="b1c46-129">Type</span><span class="sxs-lookup"><span data-stu-id="b1c46-129">Type</span></span> |<span data-ttu-id="b1c46-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c46-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1c46-131">userId</span><span class="sxs-lookup"><span data-stu-id="b1c46-131">userId</span></span>|<span data-ttu-id="b1c46-132">String</span><span class="sxs-lookup"><span data-stu-id="b1c46-132">String</span></span>|<span data-ttu-id="b1c46-133">ID do proprietário.</span><span class="sxs-lookup"><span data-stu-id="b1c46-133">ID of the owner.</span></span>|
|<span data-ttu-id="b1c46-134">type</span><span class="sxs-lookup"><span data-stu-id="b1c46-134">type</span></span>|<span data-ttu-id="b1c46-135">String</span><span class="sxs-lookup"><span data-stu-id="b1c46-135">String</span></span>|<span data-ttu-id="b1c46-136">Tipo de objetos pertencentes para retornar; `Group` atualmente é o único valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c46-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="b1c46-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c46-137">Response</span></span>

<span data-ttu-id="b1c46-138">Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto de resposta inclui propriedades do [diretório (itens excluídos)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c46-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="b1c46-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1c46-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1c46-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c46-140">Request</span></span>

<span data-ttu-id="b1c46-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1c46-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="b1c46-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c46-142">Response</span></span>

<span data-ttu-id="b1c46-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c46-143">Here is an example of the response.</span></span> <span data-ttu-id="b1c46-144">Observação: Este objeto de resposta pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="b1c46-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="b1c46-145">Todas as propriedades com suporte são retornadas de chamadas reais.</span><span class="sxs-lookup"><span data-stu-id="b1c46-145">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
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


