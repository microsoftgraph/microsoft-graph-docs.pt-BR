---
title: tipo de recurso externalConnection
description: Uma conexão é um contêiner lógico para seu conteúdo externo no Microsoft Graph
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 82a68c8670a1381263d0b6fd3704f9d6d900d1f0
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193138"
---
# <a name="externalconnection-resource-type"></a><span data-ttu-id="1bf47-103">tipo de recurso externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-103">externalConnection resource type</span></span>

<span data-ttu-id="1bf47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bf47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bf47-105">Um contêiner lógico para adicionar conteúdo de uma fonte externa no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1bf47-105">A logical container to add content from an external source into Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="1bf47-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1bf47-106">Methods</span></span>

| <span data-ttu-id="1bf47-107">Método</span><span class="sxs-lookup"><span data-stu-id="1bf47-107">Method</span></span>                                                           | <span data-ttu-id="1bf47-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1bf47-108">Return Type</span></span>                                   | <span data-ttu-id="1bf47-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bf47-109">Description</span></span> |
|:-----------------------------------------------------------------|:----------------------------------------------|:--|
| [<span data-ttu-id="1bf47-110">Criar externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-110">Create externalConnection</span></span>](../api/external-post-connections.md) | <span data-ttu-id="1bf47-111">externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-111">externalConnection</span></span>                            | <span data-ttu-id="1bf47-112">Crie um novo externalConnection postando na coleção Connections.</span><span class="sxs-lookup"><span data-stu-id="1bf47-112">Create a new externalConnection by posting to the connections collection.</span></span> |
| [<span data-ttu-id="1bf47-113">Listar externalConnections</span><span class="sxs-lookup"><span data-stu-id="1bf47-113">List externalConnections</span></span>](../api/externalconnection-list.md)    | <span data-ttu-id="1bf47-114">coleção externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-114">externalConnection collection</span></span>                 | <span data-ttu-id="1bf47-115">Obtenha uma coleção de objetos externalConnection.</span><span class="sxs-lookup"><span data-stu-id="1bf47-115">Get a externalConnection object collection.</span></span> |
| [<span data-ttu-id="1bf47-116">Obter externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-116">Get externalConnection</span></span>](../api/externalconnection-get.md)       | <span data-ttu-id="1bf47-117">externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-117">externalConnection</span></span>                            | <span data-ttu-id="1bf47-118">Ler propriedades e relações de um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="1bf47-118">Read properties and relationships of a externalConnection object.</span></span> |
| [<span data-ttu-id="1bf47-119">Atualizar externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-119">Update externalConnection</span></span>](../api/externalconnection-update.md) | <span data-ttu-id="1bf47-120">externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-120">externalConnection</span></span>                            | <span data-ttu-id="1bf47-121">Atualizar um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="1bf47-121">Update a externalConnection object.</span></span> |
| [<span data-ttu-id="1bf47-122">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="1bf47-122">Delete externalConnection</span></span>](../api/externalconnection-delete.md) | <span data-ttu-id="1bf47-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1bf47-123">None</span></span>                                          | <span data-ttu-id="1bf47-124">Excluir um objeto externalConnection.</span><span class="sxs-lookup"><span data-stu-id="1bf47-124">Delete a externalConnection object.</span></span> |
| [<span data-ttu-id="1bf47-125">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="1bf47-125">Create schema</span></span>](../api/externalconnection-post-schema.md)        | <span data-ttu-id="1bf47-126">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="1bf47-126">None *or* [schema](schema.md)</span></span>                 | <span data-ttu-id="1bf47-127">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="1bf47-127">Register connection schema.</span></span> |
| [<span data-ttu-id="1bf47-128">Operação get</span><span class="sxs-lookup"><span data-stu-id="1bf47-128">Get operation</span></span>](../api/connectionoperation-get.md)               | [<span data-ttu-id="1bf47-129">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="1bf47-129">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="1bf47-130">Obter o status de uma solicitação assíncrona para criar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="1bf47-130">Get the status of an asynchronous request to create the connection schema.</span></span> |
| [<span data-ttu-id="1bf47-131">Criar externalItem</span><span class="sxs-lookup"><span data-stu-id="1bf47-131">Create externalItem</span></span>](../api/externalconnection-put-items.md)    | [<span data-ttu-id="1bf47-132">externalItem</span><span class="sxs-lookup"><span data-stu-id="1bf47-132">externalItem</span></span>](externalitem.md)               | <span data-ttu-id="1bf47-133">Criar um novo externalItem postando na coleção Items.</span><span class="sxs-lookup"><span data-stu-id="1bf47-133">Create a new externalItem by posting to the items collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="1bf47-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bf47-134">Properties</span></span>

| <span data-ttu-id="1bf47-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bf47-135">Property</span></span>      | <span data-ttu-id="1bf47-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bf47-136">Type</span></span>                              | <span data-ttu-id="1bf47-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bf47-137">Description</span></span> |
|:--------------|:----------------------------------|:------------|
| <span data-ttu-id="1bf47-138">configuration</span><span class="sxs-lookup"><span data-stu-id="1bf47-138">configuration</span></span> | [<span data-ttu-id="1bf47-139">configuration</span><span class="sxs-lookup"><span data-stu-id="1bf47-139">configuration</span></span>](configuration.md) | <span data-ttu-id="1bf47-140">Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar o conteúdo na conexão.</span><span class="sxs-lookup"><span data-stu-id="1bf47-140">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> <span data-ttu-id="1bf47-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1bf47-141">Optional.</span></span> |
| <span data-ttu-id="1bf47-142">description</span><span class="sxs-lookup"><span data-stu-id="1bf47-142">description</span></span>   | <span data-ttu-id="1bf47-143">String</span><span class="sxs-lookup"><span data-stu-id="1bf47-143">String</span></span>                            | <span data-ttu-id="1bf47-144">Descrição da conexão exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1bf47-144">Description of the connection displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="1bf47-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1bf47-145">Optional.</span></span> |
| <span data-ttu-id="1bf47-146">id</span><span class="sxs-lookup"><span data-stu-id="1bf47-146">id</span></span>            | <span data-ttu-id="1bf47-147">String</span><span class="sxs-lookup"><span data-stu-id="1bf47-147">String</span></span>                            | <span data-ttu-id="1bf47-148">ID exclusiva fornecida pelo desenvolvedor da conexão dentro do locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1bf47-148">Developer-provided unique ID of the connection within the Azure Active Directory tenant.</span></span> <span data-ttu-id="1bf47-149">Comprimento máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1bf47-149">Maximum length of 32 characters.</span></span> <span data-ttu-id="1bf47-150">Deve conter apenas caracteres alfanuméricos.</span><span class="sxs-lookup"><span data-stu-id="1bf47-150">Must only contain alphanumeric characters.</span></span> <span data-ttu-id="1bf47-151">Não pode começar com `Microsoft` um dos seguintes valores:,, `None` `Directory` ,, `Exchange` `ExchangeArchive` `LinkedIn` , `Mailbox` , `MicrosoftSearch` , `OneDriveBusiness` ,,, `SharePoint` , `Teams` `Yammer` `Connectors` ,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="1bf47-151">Cannot begin with `Microsoft` or be one of the following values: `None`, `Directory`, `Exchange`, `ExchangeArchive`, `LinkedIn`, `Mailbox`, `MicrosoftSearch`, `OneDriveBusiness`, `SharePoint`, `Teams`, `Yammer`, `Connectors`.</span></span> <span data-ttu-id="1bf47-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bf47-152">Required.</span></span> |
| <span data-ttu-id="1bf47-153">nome</span><span class="sxs-lookup"><span data-stu-id="1bf47-153">name</span></span>          | <span data-ttu-id="1bf47-154">String</span><span class="sxs-lookup"><span data-stu-id="1bf47-154">String</span></span>                            | <span data-ttu-id="1bf47-155">O nome de exibição da conexão a ser exibida no centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1bf47-155">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="1bf47-156">Comprimento máximo de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1bf47-156">Maximum length of 128 characters.</span></span> <span data-ttu-id="1bf47-157">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bf47-157">Required.</span></span> |
| <span data-ttu-id="1bf47-158">state</span><span class="sxs-lookup"><span data-stu-id="1bf47-158">state</span></span>         | <span data-ttu-id="1bf47-159">connectionState</span><span class="sxs-lookup"><span data-stu-id="1bf47-159">connectionState</span></span>                   | <span data-ttu-id="1bf47-160">Indica o estado atual da conexão.</span><span class="sxs-lookup"><span data-stu-id="1bf47-160">Indicates the current state of the connection.</span></span> <span data-ttu-id="1bf47-161">Os valores possíveis são:,, `draft` `ready` `obsolete` e `limitExceeded` .</span><span class="sxs-lookup"><span data-stu-id="1bf47-161">Possible values are `draft`, `ready`, `obsolete`, and `limitExceeded`.</span></span> <span data-ttu-id="1bf47-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bf47-162">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1bf47-163">Relações</span><span class="sxs-lookup"><span data-stu-id="1bf47-163">Relationships</span></span>

| <span data-ttu-id="1bf47-164">Relação</span><span class="sxs-lookup"><span data-stu-id="1bf47-164">Relationship</span></span> | <span data-ttu-id="1bf47-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bf47-165">Type</span></span>                                                     | <span data-ttu-id="1bf47-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bf47-166">Description</span></span> |
|:-------------|:---------------------------------------------------------|:---|
| <span data-ttu-id="1bf47-167">items</span><span class="sxs-lookup"><span data-stu-id="1bf47-167">items</span></span>        | <span data-ttu-id="1bf47-168">coleção [externalItem](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="1bf47-168">[externalItem](externalitem.md) collection</span></span>               | <span data-ttu-id="1bf47-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1bf47-p106">Read-only. Nullable.</span></span> |
| <span data-ttu-id="1bf47-171">operations</span><span class="sxs-lookup"><span data-stu-id="1bf47-171">operations</span></span>   | <span data-ttu-id="1bf47-172">coleção [connectionOperation](connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="1bf47-172">[connectionOperation](connectionoperation.md) collection</span></span> | <span data-ttu-id="1bf47-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1bf47-173">Read-only.</span></span> <span data-ttu-id="1bf47-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1bf47-174">Nullable.</span></span> |
| <span data-ttu-id="1bf47-175">esquemas</span><span class="sxs-lookup"><span data-stu-id="1bf47-175">schema</span></span>       | [<span data-ttu-id="1bf47-176">schema</span><span class="sxs-lookup"><span data-stu-id="1bf47-176">schema</span></span>](schema.md)                                      | <span data-ttu-id="1bf47-p108">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1bf47-p108">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bf47-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bf47-179">JSON representation</span></span>

<span data-ttu-id="1bf47-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bf47-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "configuration": {"@odata.type": "microsoft.graph.configuration"},
  "description": "String",
  "id": "String (identifier)",
  "name": "String",
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
