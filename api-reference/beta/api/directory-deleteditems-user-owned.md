---
title: Permissions
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f02d6dccd005696c130c6bb4a1f42c603943e5c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960564"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="cbbe7-103">**Listar itens excluídos pertencentes a um usuário**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="cbbe7-104">Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="cbbe7-105">Atualmente, a funcionalidade de itens de lista excluída é suportada somente para [Agrupar](../resources/group.md) recursos pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="cbbe7-106">Esta é uma ação de serviço, o que significa que ele não dá suporte a paginação.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="cbbe7-107">A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificado por ID.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>  <span data-ttu-id="cbbe7-108">O usuário deve pertencer 1.000 ou mais excluído objetos, a API retorna nothing.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-108">Should the user own 1,000 or more deleted objects, the API returns nothing.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbbe7-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="cbbe7-109">Permissions</span></span>

<span data-ttu-id="cbbe7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="cbbe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="cbbe7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbbe7-112">Permission type</span></span> | <span data-ttu-id="cbbe7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbbe7-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="cbbe7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbbe7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cbbe7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbbe7-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cbbe7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbbe7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cbbe7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-117">Not supported.</span></span> |
| <span data-ttu-id="cbbe7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbbe7-118">Application</span></span> | <span data-ttu-id="cbbe7-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbbe7-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cbbe7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbbe7-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="cbbe7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbe7-121">Request headers</span></span>

| <span data-ttu-id="cbbe7-122">**Nome**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-122">**Name**</span></span>      | <span data-ttu-id="cbbe7-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-123">**Description**</span></span>           |
| ------------- | ------------------------- |
| <span data-ttu-id="cbbe7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbbe7-124">Authorization</span></span> | <span data-ttu-id="cbbe7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbbe7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbe7-127">Request body</span></span>

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

<span data-ttu-id="cbbe7-128">O corpo da solicitação requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="cbbe7-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="cbbe7-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cbbe7-129">Parameter</span></span>    | <span data-ttu-id="cbbe7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbbe7-130">Type</span></span> |<span data-ttu-id="cbbe7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbbe7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbbe7-132">userId</span><span class="sxs-lookup"><span data-stu-id="cbbe7-132">userId</span></span>|<span data-ttu-id="cbbe7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbbe7-133">String</span></span>|<span data-ttu-id="cbbe7-134">ID do proprietário.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-134">ID of the owner.</span></span>|
|<span data-ttu-id="cbbe7-135">type</span><span class="sxs-lookup"><span data-stu-id="cbbe7-135">type</span></span>|<span data-ttu-id="cbbe7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbbe7-136">String</span></span>|<span data-ttu-id="cbbe7-137">Tipo de objetos pertencentes para retornar; `Group` atualmente é o único valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-137">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|

## <a name="response"></a><span data-ttu-id="cbbe7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbbe7-138">Response</span></span>

<span data-ttu-id="cbbe7-139">Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto de resposta inclui propriedades do [diretório (itens excluídos)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="cbbe7-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="cbbe7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbbe7-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cbbe7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbbe7-141">Request</span></span>

<span data-ttu-id="cbbe7-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a><span data-ttu-id="cbbe7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbbe7-143">Response</span></span>

<span data-ttu-id="cbbe7-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-144">Here is an example of the response.</span></span> <span data-ttu-id="cbbe7-145">Observação: Este objeto de resposta pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="cbbe7-146">Todas as propriedades com suporte são retornadas de chamadas reais.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
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


