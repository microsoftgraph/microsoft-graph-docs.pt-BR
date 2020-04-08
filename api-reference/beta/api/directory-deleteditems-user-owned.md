---
title: Listar itens excluídos pertencentes a um usuário
description: 'Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.  '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebf1e51810eacbbd14fa59b7d266f2fce4969c8b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180997"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="381b7-103">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="381b7-103">List deleted items owned by a user</span></span>

<span data-ttu-id="381b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="381b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="381b7-105">Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="381b7-105">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="381b7-106">Atualmente, a funcionalidade Listar itens excluídos é suportada apenas para recursos de [aplicativo](../resources/application.md) e de [grupo](../resources/group.md) pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="381b7-106">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="381b7-107">Esta é uma ação de serviço, o que significa que ele não oferece suporte à paginação.</span><span class="sxs-lookup"><span data-stu-id="381b7-107">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="381b7-108">A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificados por ID.</span><span class="sxs-lookup"><span data-stu-id="381b7-108">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="381b7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="381b7-109">Permissions</span></span>

<span data-ttu-id="381b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="381b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="381b7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="381b7-112">Permission type</span></span> | <span data-ttu-id="381b7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="381b7-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="381b7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="381b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="381b7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="381b7-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="381b7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="381b7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="381b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="381b7-117">Not supported.</span></span> |
| <span data-ttu-id="381b7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="381b7-118">Application</span></span> | <span data-ttu-id="381b7-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="381b7-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="381b7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="381b7-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="381b7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="381b7-121">Request headers</span></span>

| <span data-ttu-id="381b7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="381b7-122">Name</span></span>          | <span data-ttu-id="381b7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="381b7-123">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="381b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="381b7-124">Authorization</span></span> | <span data-ttu-id="381b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="381b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="381b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="381b7-127">Request body</span></span>

<span data-ttu-id="381b7-128">O corpo da solicitação requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="381b7-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="381b7-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="381b7-129">Parameter</span></span>    | <span data-ttu-id="381b7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="381b7-130">Type</span></span> |<span data-ttu-id="381b7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="381b7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="381b7-132">userId</span><span class="sxs-lookup"><span data-stu-id="381b7-132">userId</span></span>|<span data-ttu-id="381b7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="381b7-133">String</span></span>|<span data-ttu-id="381b7-134">ID do proprietário.</span><span class="sxs-lookup"><span data-stu-id="381b7-134">ID of the owner.</span></span>|
|<span data-ttu-id="381b7-135">type</span><span class="sxs-lookup"><span data-stu-id="381b7-135">type</span></span>|<span data-ttu-id="381b7-136">String</span><span class="sxs-lookup"><span data-stu-id="381b7-136">String</span></span>|<span data-ttu-id="381b7-137">Tipo de objetos de propriedade a ser retornado; `group` no momento, o único valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="381b7-137">Type of owned objects to return; `group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="381b7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="381b7-138">Response</span></span>

<span data-ttu-id="381b7-139">Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto Response inclui propriedades [de diretório (itens excluídos)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="381b7-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="381b7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="381b7-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="381b7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="381b7-141">Request</span></span>

<span data-ttu-id="381b7-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="381b7-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="381b7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="381b7-143">Response</span></span>

<span data-ttu-id="381b7-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="381b7-144">Here is an example of the response.</span></span> <span data-ttu-id="381b7-145">Observação: esse objeto de resposta pode ser truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="381b7-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="381b7-146">Todas as propriedades com suporte são retornadas de chamadas reais.</span><span class="sxs-lookup"><span data-stu-id="381b7-146">All supported properties are returned from actual calls.</span></span>

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


